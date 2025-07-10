```python
import numpy as np
import matplotlib.pyplot as plt
import os
from PIL import Image
from pathlib import Path
import time
import cv2
from tensorflow.keras.models import load_model
from tensorflow.keras.preprocessing.image import img_to_array
import tensorflow as tf

# Set the output directory
desktop = Path.home() / "Desktop"
output_dir = os.path.join(desktop, "test.historical_images", "slide 31","2")
os.makedirs(output_dir, exist_ok=True)

# Microscope initial setup
pos = microscope.position
starting_pos = pos.copy()

# Define step size and image size to maintain 30% overlap
step_size = 1500  # Step size in microns
image_size = step_size / 0.70  # Image size to maintain 30% overlap

# Define the scanning area based on sample coordinates
start_x = 80797
end_x = 84797
start_y = 33472
end_y = 37472

# Calculate number of steps
num_steps_x = int(abs(end_x - start_x) / step_size) + 1
num_steps_y = int(abs(end_y - start_y) / step_size) + 1

image_paths = []  # Store captured image paths for stitching

def is_focused(image_array):
    """Check if the image is in focus based on contrast."""
    focus_metric = image_array.std()
    return focus_metric > 10  # Adjust threshold based on real images

# Zigzag scanning pattern
for y in range(num_steps_y):
    for x in range(num_steps_x):
        start_time = time.time()

        # Calculate new position
        pos['x'] = start_x + (x * step_size if y % 2 == 0 else (num_steps_x - 1 - x) * step_size)
        pos['y'] = start_y + y * step_size
        microscope.move(pos)
        assert microscope.position == pos

        time.sleep(1)  # Stabilization delay

        # Autofocus with retries
        focused = False
        for attempt in range(1):
            microscope.autofocus()
            time.sleep(1)
            image = microscope.grab_image()
            image_array = np.array(image)
            if is_focused(image_array):
                focused = True
                break

        if not focused:
            print(f"Warning: Image at ({pos['x']}, {pos['y']}) may not be in focus.")

        # Capture and save image
        image = microscope.grab_image()
        image_array = np.array(image)
        image_filename = os.path.join(output_dir, f"image_x{x}_y{y}.png")
        Image.fromarray(image_array).save(image_filename)
        image_paths.append(image_filename)

        # Display the image
        plt.figure(figsize=(5, 5))
        plt.imshow(image_array, cmap='gray')
        plt.title(f"Image x{x} y{y}")
        plt.axis("off")
        plt.show()

        end_time = time.time()
        print(f"Captured image at ({pos['x']}, {pos['y']}) in {end_time - start_time:.2f} seconds")

# Move back to starting position
microscope.move(starting_pos)
print(f"Captured {len(image_paths)} images. Now stitching all images together...")

# ------ Image Stitching Process ------
stitcher = cv2.Stitcher_create() if int(cv2.__version__.split('.')[0]) >= 4 else cv2.createStitcher()
images = [cv2.imread(img) for img in image_paths]

if any(img is None for img in images):
    print("Error: Some images could not be loaded. Check file paths and formats.")
else:
    status, stitched = stitcher.stitch(images)
    if status == cv2.Stitcher_OK:
        stitched_path = os.path.join(output_dir, "stitched_output.jpg")
        if cv2.imwrite(stitched_path, stitched):
            print(f"Final stitched image saved at {stitched_path}")
            plt.figure(figsize=(10, 5))
            plt.imshow(cv2.cvtColor(stitched, cv2.COLOR_BGR2RGB))
            plt.axis("off")
            plt.title("Final Stitched Image")
            plt.show()

            # ---- Model Prediction Section ----
            # Load your trained model
            model_path = r"C:\Users\Ezekiel\Desktop\model trained\BreakHis_ResNet50V2_epoch_16\BreakHis_ResNet50V2_epoch_16.h5"
            model = load_model(model_path)

            # Load and preprocess stitched image
            stitched_image = cv2.imread(stitched_path)
            stitched_image = cv2.resize(stitched_image, (224, 224))  # Change size if your model uses different input size
            stitched_image = img_to_array(stitched_image)
            stitched_image = np.expand_dims(stitched_image, axis=0)
            stitched_image = stitched_image / 255.0  # Normalize if your model was trained this way

            # Predict
            prediction = model.predict(stitched_image)
            predicted_class = np.argmax(prediction, axis=1)[0]
            confidence = np.max(prediction)

            # Apply threshold for decision
            if confidence > 0.6:
                print(f"Prediction: Malignant (Confidence: {confidence:.2f})")
            else:
                print(f"Prediction: Benign (Confidence: {confidence:.2f})")

        else:
            print("Failed to save the final stitched image.")
    else:
        print(f"Stitching failed with error code: {status}")

```
