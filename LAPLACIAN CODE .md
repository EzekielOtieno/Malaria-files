```python
import openflexure_microscope_client as ofm_client
```


```python
microscope = ofm_client.MicroscopeClient("192.168.0.110")

```


```python
import time
import numpy as np
import cv2
from openflexure_microscope_client import MicroscopeClient

# Connect to the microscope  # Replace with your microscope's IP address
  # Replace with actual IP address

# Autofocus parameters
coarse_step_size = 200  # Step size for coarse focus adjustments
coarse_num_steps = 10   # Number of steps to evaluate in each direction during coarse focus
fine_step_size = 50     # Step size for fine focus adjustments
fine_num_steps = 4      # Number of steps to evaluate in each direction during fine focus
settle_time = 0.2       # Time to wait after moving the microscope (in seconds)
variance_threshold = 10  # Ignore small variance changes, variance must change significantly to stop

def compute_laplacian_variance(image):
    """Calculate the variance of the Laplacian, which indicates image sharpness."""
    gray_image = cv2.cvtColor(image, cv2.COLOR_RGB2GRAY)
    laplacian = cv2.Laplacian(gray_image, cv2.CV_64F)
    variance = laplacian.var()
    return variance

def move_microscope_rel(z_delta):
    """Move the microscope relative to its current position along the Z-axis."""
    microscope.move_rel({"x": 0, "y": 0, "z": z_delta})

def capture_image():
    """Capture an image from the microscope and convert it to a NumPy array."""
    img = microscope.grab_image()
    return np.array(img)

def evaluate_focus_direction(step_size, num_steps):
    """Evaluate focus direction by moving the microscope upwards and downwards from the current position."""
    initial_z = microscope.position['z']
    variances = []

    # Evaluate upward direction
    for i in range(1, num_steps + 1):
        move_microscope_rel(step_size)
        time.sleep(settle_time)
        img = capture_image()
        variance = compute_laplacian_variance(img)
        variances.append((variance, microscope.position['z']))

    # Return to initial position
    move_microscope_rel(-step_size * num_steps)
    time.sleep(settle_time)

    # Evaluate downward direction
    for i in range(1, num_steps + 1):
        move_microscope_rel(-step_size)
        time.sleep(settle_time)
        img = capture_image()
        variance = compute_laplacian_variance(img)
        variances.append((variance, microscope.position['z']))

    # Return to initial position
    move_microscope_rel(step_size * num_steps)
    time.sleep(settle_time)

    return variances

def find_best_focus(variances):
    """Find the position with the highest variance indicating best focus."""
    best_variance, best_z = max(variances, key=lambda x: x[0])
    return best_z, best_variance

def move_towards_best_focus(direction, step_size, max_steps):
    """Move towards the best focus position in the identified direction until variance starts decreasing."""
    best_variance = -1
    best_z = microscope.position['z']
    prev_variance = -1
    peak_variance = -1
    peak_z = best_z
    steps_taken = 0
    
    # Keep moving in the identified direction until variance starts decreasing
    while steps_taken < max_steps:
        move_microscope_rel(direction * step_size)
        time.sleep(settle_time)
        img = capture_image()
        variance = compute_laplacian_variance(img)

        # Update peak variance if it's higher than the previous peak
        if variance > peak_variance:
            peak_variance = variance
            peak_z = microscope.position['z']
            prev_variance = variance  # Update previous variance to the new peak value
        elif variance < prev_variance and (prev_variance - variance) > variance_threshold:
            # Stop if variance has decreased significantly compared to previous
            break

        prev_variance = variance
        steps_taken += 1

    return peak_z, peak_variance

def coarse_focus():
    """Perform coarse focusing by evaluating the variance in both directions."""
    print("Starting coarse focus...")
    
    # First, evaluate the focus direction
    coarse_variances = evaluate_focus_direction(coarse_step_size, coarse_num_steps)
    
    # Find the direction with the maximum variance
    best_coarse_z, best_coarse_variance = find_best_focus(coarse_variances)
    
    print(f"Coarse focus completed at Z = {best_coarse_z} with variance = {best_coarse_variance}")
    
    # Determine direction (up or down)
    direction = 1 if best_coarse_z > microscope.position['z'] else -1
    
    # Move towards best focus position in the identified direction
    best_coarse_z, best_coarse_variance = move_towards_best_focus(direction, coarse_step_size, max_steps=50)
    
    print(f"Coarse focusing completed at Z = {best_coarse_z} with variance = {best_coarse_variance}")
    
    return best_coarse_z, best_coarse_variance

def fine_focus():
    """Perform fine focusing by continuously moving and evaluating variance."""
    print("Starting fine focus...")
    
    fine_variances = evaluate_focus_direction(fine_step_size, fine_num_steps)
    fine_best_z, fine_best_variance = find_best_focus(fine_variances)
    
    print(f"Fine focus completed at Z = {fine_best_z} with variance = {fine_best_variance}")
    
    # Determine direction (up or down)
    direction = 1 if fine_best_z > microscope.position['z'] else -1
    
    # Move towards best fine focus position
    fine_best_z, fine_best_variance = move_towards_best_focus(direction, fine_step_size, max_steps=30)
    
    print(f"Fine focusing completed at Z = {fine_best_z} with variance = {fine_best_variance}")
    
    return fine_best_z, fine_best_variance

def autofocus():
    """Perform the full autofocus routine (coarse and fine focus)."""
    # Coarse focus phase
    coarse_best_z, coarse_best_variance = coarse_focus()

    # Move to best coarse focus position
    move_microscope_rel(coarse_best_z - microscope.position['z'])
    time.sleep(settle_time)

    # Fine focus phase
    fine_best_z, fine_best_variance = fine_focus()

    # Move to best fine focus position
    move_microscope_rel(fine_best_z - microscope.position['z'])
    time.sleep(settle_time)

    return fine_best_z, fine_best_variance

# Run the autofocus routine
best_z, best_variance = autofocus()

```

    Starting coarse focus...
    Coarse focus completed at Z = 55054 with variance = 111.45784282365632
    Coarse focusing completed at Z = 54654 with variance = 159.55720806699122
    Starting fine focus...
    Fine focus completed at Z = 54854 with variance = 155.92605079467828
    Fine focusing completed at Z = 54954 with variance = 202.49877154380093
    


```python

```
