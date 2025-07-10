```python
import pandas as pd 

```


```python
weather=pd.read_csv('weather.csv')
```


```python
weather
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>STATION</th>
      <th>NAME</th>
      <th>DATE</th>
      <th>CLDD</th>
      <th>DP01</th>
      <th>DP10</th>
      <th>DT00</th>
      <th>DT32</th>
      <th>DX32</th>
      <th>DX70</th>
      <th>DX90</th>
      <th>EMNT</th>
      <th>EMXP</th>
      <th>EMXT</th>
      <th>HDSD</th>
      <th>HTDD</th>
      <th>PRCP</th>
      <th>TAVG</th>
      <th>TMAX</th>
      <th>TMIN</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1958-05</td>
      <td>NaN</td>
      <td>14.0</td>
      <td>10.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>1.58</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>7.60</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>1</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1958-06</td>
      <td>NaN</td>
      <td>9.0</td>
      <td>6.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>1.04</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2.61</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1958-07</td>
      <td>NaN</td>
      <td>10.0</td>
      <td>4.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>0.78</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2.29</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>3</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1958-08</td>
      <td>NaN</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>0.00</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>0.00</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>4</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1958-09</td>
      <td>NaN</td>
      <td>1.0</td>
      <td>1.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>1.06</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>1.06</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>557</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2017-07</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>47.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>54.8</td>
    </tr>
    <tr>
      <th>558</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-01</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>52.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>57.7</td>
    </tr>
    <tr>
      <th>559</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-02</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>54.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>58.9</td>
    </tr>
    <tr>
      <th>560</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-04</td>
      <td>NaN</td>
      <td>19.0</td>
      <td>10.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2.13</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>9.01</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>561</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-07</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>44.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>53.6</td>
    </tr>
  </tbody>
</table>
<p>562 rows × 20 columns</p>
</div>




```python
null_pct= weather.apply(pd.isnull).sum()/weather.shape[0]
```


```python
null_pct
```




    STATION    0.000000
    NAME       0.000000
    DATE       0.000000
    CLDD       0.975089
    DP01       0.142349
    DP10       0.142349
    DT00       0.774021
    DT32       0.774021
    DX32       0.717082
    DX70       0.717082
    DX90       0.717082
    EMNT       0.774021
    EMXP       0.142349
    EMXT       0.717082
    HDSD       0.998221
    HTDD       0.975089
    PRCP       0.142349
    TAVG       0.902135
    TMAX       0.717082
    TMIN       0.774021
    dtype: float64




```python
valid_columns = weather. columns[null_pct<.90]
```


```python
valid_columns
```




    Index(['STATION', 'NAME', 'DATE', 'DP01', 'DP10', 'DT00', 'DT32', 'DX32',
           'DX70', 'DX90', 'EMNT', 'EMXP', 'EMXT', 'PRCP', 'TMAX', 'TMIN'],
          dtype='object')




```python
weather=weather.ffill()
```


```python
weather
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>STATION</th>
      <th>NAME</th>
      <th>DATE</th>
      <th>CLDD</th>
      <th>DP01</th>
      <th>DP10</th>
      <th>DT00</th>
      <th>DT32</th>
      <th>DX32</th>
      <th>DX70</th>
      <th>DX90</th>
      <th>EMNT</th>
      <th>EMXP</th>
      <th>EMXT</th>
      <th>HDSD</th>
      <th>HTDD</th>
      <th>PRCP</th>
      <th>TAVG</th>
      <th>TMAX</th>
      <th>TMIN</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1958-05</td>
      <td>NaN</td>
      <td>14.0</td>
      <td>10.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>1.58</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>7.60</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>1</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1958-06</td>
      <td>NaN</td>
      <td>9.0</td>
      <td>6.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>1.04</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2.61</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1958-07</td>
      <td>NaN</td>
      <td>10.0</td>
      <td>4.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>0.78</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2.29</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>3</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1958-08</td>
      <td>NaN</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>0.00</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>0.00</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>4</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1958-09</td>
      <td>NaN</td>
      <td>1.0</td>
      <td>1.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>1.06</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>1.06</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>557</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2017-07</td>
      <td>124.0</td>
      <td>20.0</td>
      <td>17.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>27.0</td>
      <td>0.0</td>
      <td>47.0</td>
      <td>2.91</td>
      <td>84.0</td>
      <td>7.0</td>
      <td>0.0</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>54.8</td>
    </tr>
    <tr>
      <th>558</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-01</td>
      <td>124.0</td>
      <td>20.0</td>
      <td>17.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>27.0</td>
      <td>0.0</td>
      <td>52.0</td>
      <td>2.91</td>
      <td>84.0</td>
      <td>7.0</td>
      <td>0.0</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>57.7</td>
    </tr>
    <tr>
      <th>559</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-02</td>
      <td>124.0</td>
      <td>20.0</td>
      <td>17.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>27.0</td>
      <td>0.0</td>
      <td>54.0</td>
      <td>2.91</td>
      <td>84.0</td>
      <td>7.0</td>
      <td>0.0</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>58.9</td>
    </tr>
    <tr>
      <th>560</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-04</td>
      <td>124.0</td>
      <td>19.0</td>
      <td>10.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>27.0</td>
      <td>0.0</td>
      <td>54.0</td>
      <td>2.13</td>
      <td>84.0</td>
      <td>7.0</td>
      <td>0.0</td>
      <td>9.01</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>58.9</td>
    </tr>
    <tr>
      <th>561</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-07</td>
      <td>124.0</td>
      <td>19.0</td>
      <td>10.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>27.0</td>
      <td>0.0</td>
      <td>44.0</td>
      <td>2.13</td>
      <td>84.0</td>
      <td>7.0</td>
      <td>0.0</td>
      <td>9.01</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>53.6</td>
    </tr>
  </tbody>
</table>
<p>562 rows × 20 columns</p>
</div>




```python
weather.dropna(inplace=True)
```


```python
weather
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>STATION</th>
      <th>NAME</th>
      <th>DATE</th>
      <th>CLDD</th>
      <th>DP01</th>
      <th>DP10</th>
      <th>DT00</th>
      <th>DT32</th>
      <th>DX32</th>
      <th>DX70</th>
      <th>DX90</th>
      <th>EMNT</th>
      <th>EMXP</th>
      <th>EMXT</th>
      <th>HDSD</th>
      <th>HTDD</th>
      <th>PRCP</th>
      <th>TAVG</th>
      <th>TMAX</th>
      <th>TMIN</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>319</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-01</td>
      <td>67.0</td>
      <td>2.0</td>
      <td>2.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>29.0</td>
      <td>0.0</td>
      <td>47.0</td>
      <td>0.35</td>
      <td>85.0</td>
      <td>7.0</td>
      <td>7.0</td>
      <td>0.48</td>
      <td>67.3</td>
      <td>79.8</td>
      <td>54.7</td>
    </tr>
    <tr>
      <th>320</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-02</td>
      <td>67.0</td>
      <td>10.0</td>
      <td>9.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>25.0</td>
      <td>0.0</td>
      <td>52.0</td>
      <td>1.20</td>
      <td>84.0</td>
      <td>7.0</td>
      <td>7.0</td>
      <td>5.56</td>
      <td>68.1</td>
      <td>79.3</td>
      <td>56.9</td>
    </tr>
    <tr>
      <th>321</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-03</td>
      <td>67.0</td>
      <td>12.0</td>
      <td>6.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>29.0</td>
      <td>0.0</td>
      <td>52.0</td>
      <td>1.08</td>
      <td>85.0</td>
      <td>7.0</td>
      <td>7.0</td>
      <td>2.33</td>
      <td>68.1</td>
      <td>80.6</td>
      <td>56.9</td>
    </tr>
    <tr>
      <th>322</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-04</td>
      <td>67.0</td>
      <td>18.0</td>
      <td>14.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>27.0</td>
      <td>0.0</td>
      <td>57.0</td>
      <td>2.09</td>
      <td>82.0</td>
      <td>7.0</td>
      <td>7.0</td>
      <td>7.46</td>
      <td>67.7</td>
      <td>76.7</td>
      <td>58.8</td>
    </tr>
    <tr>
      <th>323</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-05</td>
      <td>67.0</td>
      <td>11.0</td>
      <td>6.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>27.0</td>
      <td>0.0</td>
      <td>57.0</td>
      <td>0.64</td>
      <td>82.0</td>
      <td>7.0</td>
      <td>7.0</td>
      <td>2.14</td>
      <td>67.7</td>
      <td>76.7</td>
      <td>58.8</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>557</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2017-07</td>
      <td>124.0</td>
      <td>20.0</td>
      <td>17.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>27.0</td>
      <td>0.0</td>
      <td>47.0</td>
      <td>2.91</td>
      <td>84.0</td>
      <td>7.0</td>
      <td>0.0</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>54.8</td>
    </tr>
    <tr>
      <th>558</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-01</td>
      <td>124.0</td>
      <td>20.0</td>
      <td>17.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>27.0</td>
      <td>0.0</td>
      <td>52.0</td>
      <td>2.91</td>
      <td>84.0</td>
      <td>7.0</td>
      <td>0.0</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>57.7</td>
    </tr>
    <tr>
      <th>559</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-02</td>
      <td>124.0</td>
      <td>20.0</td>
      <td>17.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>27.0</td>
      <td>0.0</td>
      <td>54.0</td>
      <td>2.91</td>
      <td>84.0</td>
      <td>7.0</td>
      <td>0.0</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>58.9</td>
    </tr>
    <tr>
      <th>560</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-04</td>
      <td>124.0</td>
      <td>19.0</td>
      <td>10.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>27.0</td>
      <td>0.0</td>
      <td>54.0</td>
      <td>2.13</td>
      <td>84.0</td>
      <td>7.0</td>
      <td>0.0</td>
      <td>9.01</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>58.9</td>
    </tr>
    <tr>
      <th>561</th>
      <td>KE000063740</td>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-07</td>
      <td>124.0</td>
      <td>19.0</td>
      <td>10.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>27.0</td>
      <td>0.0</td>
      <td>44.0</td>
      <td>2.13</td>
      <td>84.0</td>
      <td>7.0</td>
      <td>0.0</td>
      <td>9.01</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>53.6</td>
    </tr>
  </tbody>
</table>
<p>243 rows × 20 columns</p>
</div>




```python
start_index = 1
end_index = 19

# Use slicing to keep the specified columns
weather = weather.iloc[:, start_index:end_index+1]  
```


```python
weather
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>NAME</th>
      <th>DATE</th>
      <th>CLDD</th>
      <th>DP01</th>
      <th>DP10</th>
      <th>DT00</th>
      <th>DT32</th>
      <th>DX32</th>
      <th>DX70</th>
      <th>DX90</th>
      <th>EMNT</th>
      <th>EMXP</th>
      <th>EMXT</th>
      <th>HDSD</th>
      <th>HTDD</th>
      <th>PRCP</th>
      <th>TAVG</th>
      <th>TMAX</th>
      <th>TMIN</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>319</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-01</td>
      <td>67.0</td>
      <td>2.0</td>
      <td>2.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>29.0</td>
      <td>0.0</td>
      <td>47.0</td>
      <td>0.35</td>
      <td>85.0</td>
      <td>7.0</td>
      <td>7.0</td>
      <td>0.48</td>
      <td>67.3</td>
      <td>79.8</td>
      <td>54.7</td>
    </tr>
    <tr>
      <th>320</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-02</td>
      <td>67.0</td>
      <td>10.0</td>
      <td>9.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>25.0</td>
      <td>0.0</td>
      <td>52.0</td>
      <td>1.20</td>
      <td>84.0</td>
      <td>7.0</td>
      <td>7.0</td>
      <td>5.56</td>
      <td>68.1</td>
      <td>79.3</td>
      <td>56.9</td>
    </tr>
    <tr>
      <th>321</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-03</td>
      <td>67.0</td>
      <td>12.0</td>
      <td>6.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>29.0</td>
      <td>0.0</td>
      <td>52.0</td>
      <td>1.08</td>
      <td>85.0</td>
      <td>7.0</td>
      <td>7.0</td>
      <td>2.33</td>
      <td>68.1</td>
      <td>80.6</td>
      <td>56.9</td>
    </tr>
    <tr>
      <th>322</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-04</td>
      <td>67.0</td>
      <td>18.0</td>
      <td>14.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>27.0</td>
      <td>0.0</td>
      <td>57.0</td>
      <td>2.09</td>
      <td>82.0</td>
      <td>7.0</td>
      <td>7.0</td>
      <td>7.46</td>
      <td>67.7</td>
      <td>76.7</td>
      <td>58.8</td>
    </tr>
    <tr>
      <th>323</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-05</td>
      <td>67.0</td>
      <td>11.0</td>
      <td>6.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>27.0</td>
      <td>0.0</td>
      <td>57.0</td>
      <td>0.64</td>
      <td>82.0</td>
      <td>7.0</td>
      <td>7.0</td>
      <td>2.14</td>
      <td>67.7</td>
      <td>76.7</td>
      <td>58.8</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>557</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2017-07</td>
      <td>124.0</td>
      <td>20.0</td>
      <td>17.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>27.0</td>
      <td>0.0</td>
      <td>47.0</td>
      <td>2.91</td>
      <td>84.0</td>
      <td>7.0</td>
      <td>0.0</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>54.8</td>
    </tr>
    <tr>
      <th>558</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-01</td>
      <td>124.0</td>
      <td>20.0</td>
      <td>17.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>27.0</td>
      <td>0.0</td>
      <td>52.0</td>
      <td>2.91</td>
      <td>84.0</td>
      <td>7.0</td>
      <td>0.0</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>57.7</td>
    </tr>
    <tr>
      <th>559</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-02</td>
      <td>124.0</td>
      <td>20.0</td>
      <td>17.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>27.0</td>
      <td>0.0</td>
      <td>54.0</td>
      <td>2.91</td>
      <td>84.0</td>
      <td>7.0</td>
      <td>0.0</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>58.9</td>
    </tr>
    <tr>
      <th>560</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-04</td>
      <td>124.0</td>
      <td>19.0</td>
      <td>10.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>27.0</td>
      <td>0.0</td>
      <td>54.0</td>
      <td>2.13</td>
      <td>84.0</td>
      <td>7.0</td>
      <td>0.0</td>
      <td>9.01</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>58.9</td>
    </tr>
    <tr>
      <th>561</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-07</td>
      <td>124.0</td>
      <td>19.0</td>
      <td>10.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>27.0</td>
      <td>0.0</td>
      <td>44.0</td>
      <td>2.13</td>
      <td>84.0</td>
      <td>7.0</td>
      <td>0.0</td>
      <td>9.01</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>53.6</td>
    </tr>
  </tbody>
</table>
<p>243 rows × 19 columns</p>
</div>




```python
columns_to_drop = ['CLDD',	'DP01',	'DP10',	'DT00',	'DT32',	'DX32',	'DX70',	'DX90',	'EMNT',	'EMXP',	'EMXT',	'HDSD',	'HTDD']
weather = weather.drop(columns_to_drop, axis=1)
```


```python
weather
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>NAME</th>
      <th>DATE</th>
      <th>PRCP</th>
      <th>TAVG</th>
      <th>TMAX</th>
      <th>TMIN</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>319</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-01</td>
      <td>0.48</td>
      <td>67.3</td>
      <td>79.8</td>
      <td>54.7</td>
    </tr>
    <tr>
      <th>320</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-02</td>
      <td>5.56</td>
      <td>68.1</td>
      <td>79.3</td>
      <td>56.9</td>
    </tr>
    <tr>
      <th>321</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-03</td>
      <td>2.33</td>
      <td>68.1</td>
      <td>80.6</td>
      <td>56.9</td>
    </tr>
    <tr>
      <th>322</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-04</td>
      <td>7.46</td>
      <td>67.7</td>
      <td>76.7</td>
      <td>58.8</td>
    </tr>
    <tr>
      <th>323</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-05</td>
      <td>2.14</td>
      <td>67.7</td>
      <td>76.7</td>
      <td>58.8</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>557</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2017-07</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>54.8</td>
    </tr>
    <tr>
      <th>558</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-01</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>57.7</td>
    </tr>
    <tr>
      <th>559</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-02</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>58.9</td>
    </tr>
    <tr>
      <th>560</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-04</td>
      <td>9.01</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>58.9</td>
    </tr>
    <tr>
      <th>561</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-07</td>
      <td>9.01</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>53.6</td>
    </tr>
  </tbody>
</table>
<p>243 rows × 6 columns</p>
</div>




```python
column_means = weather[['TMAX', 'TMIN', 'PRCP','TAVG']].mean()

```


```python
column_means
```




    TMAX    78.524280
    TMIN    55.939506
    PRCP     4.563169
    TAVG    67.771193
    dtype: float64




```python
weather['DATE'] = pd.to_datetime(weather['DATE'])

start_date = pd.to_datetime('2017-01-01')
end_date = pd.to_datetime('2017-12-30')

selected_rows = weather[(weather['DATE'] >= start_date) & (weather['DATE'] <= end_date)]

selected_columns = ['TMAX', 'TMIN', 'PRCP','TAVG']
column_means = selected_rows[selected_columns].mean()

print("Column Means:")
print(column_means)

```

    Column Means:
    TMAX    79.100000
    TMIN    57.266667
    PRCP    10.750000
    TAVG    69.500000
    dtype: float64
    


```python
weather['DATE'] = pd.to_datetime(weather['DATE'])

start_date = pd.to_datetime('2013-01-01')
end_date = pd.to_datetime('2013-12-30')

selected_rows = weather[(weather['DATE'] >= start_date) & (weather['DATE'] <= end_date)]

selected_columns = ['TMAX', 'TMIN', 'PRCP','TAVG']
column_means = selected_rows[selected_columns].mean()

print("Column Means:")
print(column_means)

```

    Column Means:
    TMAX    80.50
    TMIN    55.80
    PRCP    10.75
    TAVG    70.20
    dtype: float64
    


```python
weather['DATE'] = pd.to_datetime(weather['DATE'])

start_date = pd.to_datetime('2018-01-01')
end_date = pd.to_datetime('2018-12-30')

selected_rows = weather[(weather['DATE'] >= start_date) & (weather['DATE'] <= end_date)]

selected_columns = ['TMAX', 'TMIN', 'PRCP','TAVG']
column_means = selected_rows[selected_columns].mean()

print("Column Means:")
print(column_means)

```

    Column Means:
    TMAX    79.100
    TMIN    57.275
    PRCP     9.880
    TAVG    69.500
    dtype: float64
    


```python
weather['DATE'] = pd.to_datetime(weather['DATE'])

start_date = pd.to_datetime('2016-01-01')
end_date = pd.to_datetime('2016-12-30')

selected_rows = weather[(weather['DATE'] >= start_date) & (weather['DATE'] <= end_date)]

selected_columns = ['TMAX', 'TMIN', 'PRCP','TAVG']
column_means = selected_rows[selected_columns].mean()

print("Column Means:")
print(column_means)

```

    Column Means:
    TMAX    79.10
    TMIN    54.50
    PRCP    10.75
    TAVG    69.50
    dtype: float64
    


```python
weather['DATE'] = pd.to_datetime(weather['DATE'])

start_date = pd.to_datetime('2015-01-01')
end_date = pd.to_datetime('2015-12-30')

selected_rows = weather[(weather['DATE'] >= start_date) & (weather['DATE'] <= end_date)]

selected_columns = ['TMAX', 'TMIN', 'PRCP','TAVG']
column_means = selected_rows[selected_columns].mean()

print("Column Means:")
print(column_means)

```

    Column Means:
    TMAX    83.125
    TMIN    58.825
    PRCP    10.750
    TAVG    71.125
    dtype: float64
    


```python
weather['DATE'] = pd.to_datetime(weather['DATE'])

start_date = pd.to_datetime('2011-01-01')
end_date = pd.to_datetime('2011-12-30')

selected_rows = weather[(weather['DATE'] >= start_date) & (weather['DATE'] <= end_date)]

selected_columns = ['TMAX', 'TMIN', 'PRCP','TAVG']
column_means = selected_rows[selected_columns].mean()

print("Column Means:")
print(column_means)

```

    Column Means:
    TMAX    80.266667
    TMIN    58.566667
    PRCP     9.730000
    TAVG    70.300000
    dtype: float64
    


```python
weather.head(50)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>NAME</th>
      <th>DATE</th>
      <th>PRCP</th>
      <th>TAVG</th>
      <th>TMAX</th>
      <th>TMIN</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>319</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-01-01</td>
      <td>0.48</td>
      <td>67.3</td>
      <td>79.8</td>
      <td>54.7</td>
    </tr>
    <tr>
      <th>320</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-02-01</td>
      <td>5.56</td>
      <td>68.1</td>
      <td>79.3</td>
      <td>56.9</td>
    </tr>
    <tr>
      <th>321</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-03-01</td>
      <td>2.33</td>
      <td>68.1</td>
      <td>80.6</td>
      <td>56.9</td>
    </tr>
    <tr>
      <th>322</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-04-01</td>
      <td>7.46</td>
      <td>67.7</td>
      <td>76.7</td>
      <td>58.8</td>
    </tr>
    <tr>
      <th>323</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-05-01</td>
      <td>2.14</td>
      <td>67.7</td>
      <td>76.7</td>
      <td>58.8</td>
    </tr>
    <tr>
      <th>324</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-06-01</td>
      <td>0.66</td>
      <td>67.7</td>
      <td>72.8</td>
      <td>58.8</td>
    </tr>
    <tr>
      <th>325</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-07-01</td>
      <td>0.32</td>
      <td>67.7</td>
      <td>72.8</td>
      <td>58.8</td>
    </tr>
    <tr>
      <th>326</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-08-01</td>
      <td>0.05</td>
      <td>67.7</td>
      <td>73.4</td>
      <td>58.8</td>
    </tr>
    <tr>
      <th>327</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-09-01</td>
      <td>0.67</td>
      <td>67.7</td>
      <td>73.4</td>
      <td>58.8</td>
    </tr>
    <tr>
      <th>328</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-10-01</td>
      <td>1.38</td>
      <td>67.6</td>
      <td>80.6</td>
      <td>54.5</td>
    </tr>
    <tr>
      <th>329</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-11-01</td>
      <td>1.81</td>
      <td>67.6</td>
      <td>80.6</td>
      <td>56.2</td>
    </tr>
    <tr>
      <th>330</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-12-01</td>
      <td>4.68</td>
      <td>67.6</td>
      <td>80.6</td>
      <td>55.5</td>
    </tr>
    <tr>
      <th>331</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1986-01-01</td>
      <td>1.37</td>
      <td>67.6</td>
      <td>80.9</td>
      <td>55.5</td>
    </tr>
    <tr>
      <th>332</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1986-02-01</td>
      <td>0.00</td>
      <td>69.0</td>
      <td>85.0</td>
      <td>53.0</td>
    </tr>
    <tr>
      <th>333</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1986-03-01</td>
      <td>4.41</td>
      <td>69.0</td>
      <td>85.0</td>
      <td>53.0</td>
    </tr>
    <tr>
      <th>334</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1986-04-01</td>
      <td>9.65</td>
      <td>69.0</td>
      <td>77.5</td>
      <td>53.0</td>
    </tr>
    <tr>
      <th>335</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1986-05-01</td>
      <td>6.61</td>
      <td>69.0</td>
      <td>77.5</td>
      <td>53.0</td>
    </tr>
    <tr>
      <th>336</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1986-06-01</td>
      <td>0.44</td>
      <td>69.0</td>
      <td>71.8</td>
      <td>53.0</td>
    </tr>
    <tr>
      <th>337</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1986-07-01</td>
      <td>0.00</td>
      <td>61.4</td>
      <td>73.4</td>
      <td>49.3</td>
    </tr>
    <tr>
      <th>338</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1986-08-01</td>
      <td>0.09</td>
      <td>61.4</td>
      <td>73.4</td>
      <td>49.3</td>
    </tr>
    <tr>
      <th>339</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1986-09-01</td>
      <td>0.06</td>
      <td>61.4</td>
      <td>73.4</td>
      <td>52.3</td>
    </tr>
    <tr>
      <th>340</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1986-10-01</td>
      <td>0.12</td>
      <td>61.4</td>
      <td>82.3</td>
      <td>52.3</td>
    </tr>
    <tr>
      <th>341</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1986-11-01</td>
      <td>5.53</td>
      <td>61.4</td>
      <td>82.3</td>
      <td>52.3</td>
    </tr>
    <tr>
      <th>342</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1986-12-01</td>
      <td>3.55</td>
      <td>61.4</td>
      <td>82.3</td>
      <td>52.3</td>
    </tr>
    <tr>
      <th>343</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1987-01-01</td>
      <td>0.85</td>
      <td>61.4</td>
      <td>82.3</td>
      <td>52.3</td>
    </tr>
    <tr>
      <th>344</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1987-02-01</td>
      <td>0.33</td>
      <td>61.4</td>
      <td>83.7</td>
      <td>52.3</td>
    </tr>
    <tr>
      <th>345</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1987-03-01</td>
      <td>0.28</td>
      <td>61.4</td>
      <td>83.7</td>
      <td>52.3</td>
    </tr>
    <tr>
      <th>346</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1987-04-01</td>
      <td>4.72</td>
      <td>61.4</td>
      <td>83.7</td>
      <td>52.3</td>
    </tr>
    <tr>
      <th>347</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1987-05-01</td>
      <td>3.65</td>
      <td>61.4</td>
      <td>83.7</td>
      <td>52.3</td>
    </tr>
    <tr>
      <th>348</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1987-06-01</td>
      <td>3.09</td>
      <td>61.4</td>
      <td>83.7</td>
      <td>52.3</td>
    </tr>
    <tr>
      <th>349</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1987-07-01</td>
      <td>0.02</td>
      <td>61.4</td>
      <td>83.7</td>
      <td>52.3</td>
    </tr>
    <tr>
      <th>350</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1987-08-01</td>
      <td>0.65</td>
      <td>61.4</td>
      <td>83.7</td>
      <td>52.6</td>
    </tr>
    <tr>
      <th>351</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1987-09-01</td>
      <td>0.35</td>
      <td>61.4</td>
      <td>83.7</td>
      <td>52.6</td>
    </tr>
    <tr>
      <th>352</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1987-10-01</td>
      <td>0.00</td>
      <td>69.9</td>
      <td>83.8</td>
      <td>55.9</td>
    </tr>
    <tr>
      <th>353</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1987-11-01</td>
      <td>2.50</td>
      <td>68.4</td>
      <td>79.2</td>
      <td>57.6</td>
    </tr>
    <tr>
      <th>354</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1987-12-01</td>
      <td>0.85</td>
      <td>68.4</td>
      <td>79.2</td>
      <td>57.6</td>
    </tr>
    <tr>
      <th>355</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1988-01-01</td>
      <td>1.83</td>
      <td>69.3</td>
      <td>82.5</td>
      <td>56.0</td>
    </tr>
    <tr>
      <th>356</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1988-02-01</td>
      <td>0.06</td>
      <td>69.3</td>
      <td>84.8</td>
      <td>56.0</td>
    </tr>
    <tr>
      <th>357</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1988-03-01</td>
      <td>5.78</td>
      <td>69.3</td>
      <td>83.7</td>
      <td>56.0</td>
    </tr>
    <tr>
      <th>358</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1988-04-01</td>
      <td>8.80</td>
      <td>69.3</td>
      <td>77.6</td>
      <td>56.0</td>
    </tr>
    <tr>
      <th>359</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1988-05-01</td>
      <td>2.07</td>
      <td>69.3</td>
      <td>75.9</td>
      <td>56.0</td>
    </tr>
    <tr>
      <th>360</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1988-06-01</td>
      <td>0.91</td>
      <td>69.3</td>
      <td>75.9</td>
      <td>56.0</td>
    </tr>
    <tr>
      <th>361</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1988-07-01</td>
      <td>0.20</td>
      <td>69.3</td>
      <td>75.9</td>
      <td>56.0</td>
    </tr>
    <tr>
      <th>362</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1988-08-01</td>
      <td>0.17</td>
      <td>69.3</td>
      <td>75.9</td>
      <td>56.0</td>
    </tr>
    <tr>
      <th>363</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1988-09-01</td>
      <td>0.81</td>
      <td>69.3</td>
      <td>77.7</td>
      <td>56.0</td>
    </tr>
    <tr>
      <th>364</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1988-10-01</td>
      <td>1.82</td>
      <td>69.3</td>
      <td>77.7</td>
      <td>54.6</td>
    </tr>
    <tr>
      <th>365</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1988-11-01</td>
      <td>2.26</td>
      <td>69.3</td>
      <td>76.5</td>
      <td>54.6</td>
    </tr>
    <tr>
      <th>366</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1988-12-01</td>
      <td>3.44</td>
      <td>69.3</td>
      <td>77.3</td>
      <td>54.6</td>
    </tr>
    <tr>
      <th>367</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1989-01-01</td>
      <td>4.26</td>
      <td>69.3</td>
      <td>77.3</td>
      <td>56.2</td>
    </tr>
    <tr>
      <th>368</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1989-02-01</td>
      <td>1.19</td>
      <td>69.3</td>
      <td>80.3</td>
      <td>56.2</td>
    </tr>
  </tbody>
</table>
</div>




```python
weather.shape
```




    (243, 6)




```python

```


```python
weather.info()

```

    <class 'pandas.core.frame.DataFrame'>
    Index: 243 entries, 319 to 561
    Data columns (total 6 columns):
     #   Column  Non-Null Count  Dtype         
    ---  ------  --------------  -----         
     0   NAME    243 non-null    object        
     1   DATE    243 non-null    datetime64[ns]
     2   PRCP    243 non-null    float64       
     3   TAVG    243 non-null    float64       
     4   TMAX    243 non-null    float64       
     5   TMIN    243 non-null    float64       
    dtypes: datetime64[ns](1), float64(4), object(1)
    memory usage: 13.3+ KB
    


```python
pip install tensorflow
```

    Requirement already satisfied: tensorflow in c:\users\ezekiel\anaconda3\lib\site-packages (2.16.1)
    Requirement already satisfied: tensorflow-intel==2.16.1 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow) (2.16.1)
    Requirement already satisfied: absl-py>=1.0.0 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (2.1.0)
    Requirement already satisfied: astunparse>=1.6.0 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (1.6.3)
    Requirement already satisfied: flatbuffers>=23.5.26 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (24.3.25)
    Requirement already satisfied: gast!=0.5.0,!=0.5.1,!=0.5.2,>=0.2.1 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (0.5.4)
    Requirement already satisfied: google-pasta>=0.1.1 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (0.2.0)
    Requirement already satisfied: h5py>=3.10.0 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (3.11.0)
    Requirement already satisfied: libclang>=13.0.0 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (18.1.1)
    Requirement already satisfied: ml-dtypes~=0.3.1 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (0.3.2)
    Requirement already satisfied: opt-einsum>=2.3.2 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (3.3.0)
    Requirement already satisfied: packaging in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (23.1)
    Requirement already satisfied: protobuf!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0dev,>=3.20.3 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (3.20.3)
    Requirement already satisfied: requests<3,>=2.21.0 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (2.31.0)
    Requirement already satisfied: setuptools in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (68.2.2)
    Requirement already satisfied: six>=1.12.0 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (1.16.0)
    Requirement already satisfied: termcolor>=1.1.0 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (2.4.0)
    Requirement already satisfied: typing-extensions>=3.6.6 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (4.9.0)
    Requirement already satisfied: wrapt>=1.11.0 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (1.14.1)
    Requirement already satisfied: grpcio<2.0,>=1.24.3 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (1.64.0)
    Requirement already satisfied: tensorboard<2.17,>=2.16 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (2.16.2)
    Requirement already satisfied: keras>=3.0.0 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (3.3.3)
    Requirement already satisfied: tensorflow-io-gcs-filesystem>=0.23.1 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (0.31.0)
    Requirement already satisfied: numpy<2.0.0,>=1.23.5 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorflow-intel==2.16.1->tensorflow) (1.26.4)
    Requirement already satisfied: wheel<1.0,>=0.23.0 in c:\users\ezekiel\anaconda3\lib\site-packages (from astunparse>=1.6.0->tensorflow-intel==2.16.1->tensorflow) (0.41.2)
    Requirement already satisfied: rich in c:\users\ezekiel\anaconda3\lib\site-packages (from keras>=3.0.0->tensorflow-intel==2.16.1->tensorflow) (13.3.5)
    Requirement already satisfied: namex in c:\users\ezekiel\anaconda3\lib\site-packages (from keras>=3.0.0->tensorflow-intel==2.16.1->tensorflow) (0.0.8)
    Requirement already satisfied: optree in c:\users\ezekiel\anaconda3\lib\site-packages (from keras>=3.0.0->tensorflow-intel==2.16.1->tensorflow) (0.11.0)
    Requirement already satisfied: charset-normalizer<4,>=2 in c:\users\ezekiel\anaconda3\lib\site-packages (from requests<3,>=2.21.0->tensorflow-intel==2.16.1->tensorflow) (2.0.4)
    Requirement already satisfied: idna<4,>=2.5 in c:\users\ezekiel\anaconda3\lib\site-packages (from requests<3,>=2.21.0->tensorflow-intel==2.16.1->tensorflow) (3.4)
    Requirement already satisfied: urllib3<3,>=1.21.1 in c:\users\ezekiel\anaconda3\lib\site-packages (from requests<3,>=2.21.0->tensorflow-intel==2.16.1->tensorflow) (2.0.7)
    Requirement already satisfied: certifi>=2017.4.17 in c:\users\ezekiel\anaconda3\lib\site-packages (from requests<3,>=2.21.0->tensorflow-intel==2.16.1->tensorflow) (2024.2.2)
    Requirement already satisfied: markdown>=2.6.8 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorboard<2.17,>=2.16->tensorflow-intel==2.16.1->tensorflow) (3.4.1)
    Requirement already satisfied: tensorboard-data-server<0.8.0,>=0.7.0 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorboard<2.17,>=2.16->tensorflow-intel==2.16.1->tensorflow) (0.7.2)
    Requirement already satisfied: werkzeug>=1.0.1 in c:\users\ezekiel\anaconda3\lib\site-packages (from tensorboard<2.17,>=2.16->tensorflow-intel==2.16.1->tensorflow) (2.2.3)
    Requirement already satisfied: MarkupSafe>=2.1.1 in c:\users\ezekiel\anaconda3\lib\site-packages (from werkzeug>=1.0.1->tensorboard<2.17,>=2.16->tensorflow-intel==2.16.1->tensorflow) (2.1.3)
    Requirement already satisfied: markdown-it-py<3.0.0,>=2.2.0 in c:\users\ezekiel\anaconda3\lib\site-packages (from rich->keras>=3.0.0->tensorflow-intel==2.16.1->tensorflow) (2.2.0)
    Requirement already satisfied: pygments<3.0.0,>=2.13.0 in c:\users\ezekiel\anaconda3\lib\site-packages (from rich->keras>=3.0.0->tensorflow-intel==2.16.1->tensorflow) (2.15.1)
    Requirement already satisfied: mdurl~=0.1 in c:\users\ezekiel\anaconda3\lib\site-packages (from markdown-it-py<3.0.0,>=2.2.0->rich->keras>=3.0.0->tensorflow-intel==2.16.1->tensorflow) (0.1.0)
    Note: you may need to restart the kernel to use updated packages.
    


```python

```


```python
data= weather
```


```python
data
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>NAME</th>
      <th>DATE</th>
      <th>PRCP</th>
      <th>TAVG</th>
      <th>TMAX</th>
      <th>TMIN</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>319</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-01-01</td>
      <td>0.48</td>
      <td>67.3</td>
      <td>79.8</td>
      <td>54.7</td>
    </tr>
    <tr>
      <th>320</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-02-01</td>
      <td>5.56</td>
      <td>68.1</td>
      <td>79.3</td>
      <td>56.9</td>
    </tr>
    <tr>
      <th>321</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-03-01</td>
      <td>2.33</td>
      <td>68.1</td>
      <td>80.6</td>
      <td>56.9</td>
    </tr>
    <tr>
      <th>322</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-04-01</td>
      <td>7.46</td>
      <td>67.7</td>
      <td>76.7</td>
      <td>58.8</td>
    </tr>
    <tr>
      <th>323</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-05-01</td>
      <td>2.14</td>
      <td>67.7</td>
      <td>76.7</td>
      <td>58.8</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>557</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2017-07-01</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>54.8</td>
    </tr>
    <tr>
      <th>558</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-01-01</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>57.7</td>
    </tr>
    <tr>
      <th>559</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-02-01</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>58.9</td>
    </tr>
    <tr>
      <th>560</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-04-01</td>
      <td>9.01</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>58.9</td>
    </tr>
    <tr>
      <th>561</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-07-01</td>
      <td>9.01</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>53.6</td>
    </tr>
  </tbody>
</table>
<p>243 rows × 6 columns</p>
</div>




```python
print(data.isnull().sum())

```

    NAME    0
    DATE    0
    PRCP    0
    TAVG    0
    TMAX    0
    TMIN    0
    dtype: int64
    


```python
data.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>NAME</th>
      <th>DATE</th>
      <th>PRCP</th>
      <th>TAVG</th>
      <th>TMAX</th>
      <th>TMIN</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>319</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-01-01</td>
      <td>0.48</td>
      <td>67.3</td>
      <td>79.8</td>
      <td>54.7</td>
    </tr>
    <tr>
      <th>320</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-02-01</td>
      <td>5.56</td>
      <td>68.1</td>
      <td>79.3</td>
      <td>56.9</td>
    </tr>
    <tr>
      <th>321</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-03-01</td>
      <td>2.33</td>
      <td>68.1</td>
      <td>80.6</td>
      <td>56.9</td>
    </tr>
    <tr>
      <th>322</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-04-01</td>
      <td>7.46</td>
      <td>67.7</td>
      <td>76.7</td>
      <td>58.8</td>
    </tr>
    <tr>
      <th>323</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-05-01</td>
      <td>2.14</td>
      <td>67.7</td>
      <td>76.7</td>
      <td>58.8</td>
    </tr>
  </tbody>
</table>
</div>




```python
data.info()
```

    <class 'pandas.core.frame.DataFrame'>
    Index: 243 entries, 319 to 561
    Data columns (total 6 columns):
     #   Column  Non-Null Count  Dtype         
    ---  ------  --------------  -----         
     0   NAME    243 non-null    object        
     1   DATE    243 non-null    datetime64[ns]
     2   PRCP    243 non-null    float64       
     3   TAVG    243 non-null    float64       
     4   TMAX    243 non-null    float64       
     5   TMIN    243 non-null    float64       
    dtypes: datetime64[ns](1), float64(4), object(1)
    memory usage: 13.3+ KB
    


```python
data.dropna(inplace=True)
```


```python
data
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>NAME</th>
      <th>DATE</th>
      <th>PRCP</th>
      <th>TAVG</th>
      <th>TMAX</th>
      <th>TMIN</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>319</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-01-01</td>
      <td>0.48</td>
      <td>67.3</td>
      <td>79.8</td>
      <td>54.7</td>
    </tr>
    <tr>
      <th>320</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-02-01</td>
      <td>5.56</td>
      <td>68.1</td>
      <td>79.3</td>
      <td>56.9</td>
    </tr>
    <tr>
      <th>321</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-03-01</td>
      <td>2.33</td>
      <td>68.1</td>
      <td>80.6</td>
      <td>56.9</td>
    </tr>
    <tr>
      <th>322</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-04-01</td>
      <td>7.46</td>
      <td>67.7</td>
      <td>76.7</td>
      <td>58.8</td>
    </tr>
    <tr>
      <th>323</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>1985-05-01</td>
      <td>2.14</td>
      <td>67.7</td>
      <td>76.7</td>
      <td>58.8</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>557</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2017-07-01</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>54.8</td>
    </tr>
    <tr>
      <th>558</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-01-01</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>57.7</td>
    </tr>
    <tr>
      <th>559</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-02-01</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>58.9</td>
    </tr>
    <tr>
      <th>560</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-04-01</td>
      <td>9.01</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>58.9</td>
    </tr>
    <tr>
      <th>561</th>
      <td>JOMO KENYATTA INTERNATIONAL, KE</td>
      <td>2018-07-01</td>
      <td>9.01</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>53.6</td>
    </tr>
  </tbody>
</table>
<p>243 rows × 6 columns</p>
</div>




```python
nan_check = data.isna().any().any()
print(nan_check)

```

    False
    


```python



nan_values = data.isna().sum()
print(nan_values)

```

    NAME    0
    DATE    0
    PRCP    0
    TAVG    0
    TMAX    0
    TMIN    0
    dtype: int64
    


```python
columns_to_drop = ['NAME']
data = data.drop(columns_to_drop, axis=1)
```


```python
data
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>DATE</th>
      <th>PRCP</th>
      <th>TAVG</th>
      <th>TMAX</th>
      <th>TMIN</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>319</th>
      <td>1985-01-01</td>
      <td>0.48</td>
      <td>67.3</td>
      <td>79.8</td>
      <td>54.7</td>
    </tr>
    <tr>
      <th>320</th>
      <td>1985-02-01</td>
      <td>5.56</td>
      <td>68.1</td>
      <td>79.3</td>
      <td>56.9</td>
    </tr>
    <tr>
      <th>321</th>
      <td>1985-03-01</td>
      <td>2.33</td>
      <td>68.1</td>
      <td>80.6</td>
      <td>56.9</td>
    </tr>
    <tr>
      <th>322</th>
      <td>1985-04-01</td>
      <td>7.46</td>
      <td>67.7</td>
      <td>76.7</td>
      <td>58.8</td>
    </tr>
    <tr>
      <th>323</th>
      <td>1985-05-01</td>
      <td>2.14</td>
      <td>67.7</td>
      <td>76.7</td>
      <td>58.8</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>557</th>
      <td>2017-07-01</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>54.8</td>
    </tr>
    <tr>
      <th>558</th>
      <td>2018-01-01</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>57.7</td>
    </tr>
    <tr>
      <th>559</th>
      <td>2018-02-01</td>
      <td>10.75</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>58.9</td>
    </tr>
    <tr>
      <th>560</th>
      <td>2018-04-01</td>
      <td>9.01</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>58.9</td>
    </tr>
    <tr>
      <th>561</th>
      <td>2018-07-01</td>
      <td>9.01</td>
      <td>69.5</td>
      <td>79.1</td>
      <td>53.6</td>
    </tr>
  </tbody>
</table>
<p>243 rows × 5 columns</p>
</div>




```python
weather['DATE'] = pd.to_datetime(weather['DATE'])

start_date = pd.to_datetime('2014-01-01')
end_date = pd.to_datetime('2014-12-30')

selected_rows = weather[(weather['DATE'] >= start_date) & (weather['DATE'] <= end_date)]

selected_columns = ['TMAX', 'TMIN', 'PRCP','TAVG']
column_means = selected_rows[selected_columns].mean()

print("Column Means:")
print(column_means)

```

    Column Means:
    TMAX    80.300
    TMIN    55.725
    PRCP    10.750
    TAVG    70.200
    dtype: float64
    


```python
weather['DATE'] = pd.to_datetime(weather['DATE'])

start_date = pd.to_datetime('2012-01-01')
end_date = pd.to_datetime('2012-12-30')

selected_rows = weather[(weather['DATE'] >= start_date) & (weather['DATE'] <= end_date)]

selected_columns = ['TMAX', 'TMIN', 'PRCP','TAVG']
column_means = selected_rows[selected_columns].mean()

print("Column Means:")
print(column_means)

```

    Column Means:
    TMAX    79.10
    TMIN    59.20
    PRCP    10.75
    TAVG    70.20
    dtype: float64
    


```python
weather['DATE'] = pd.to_datetime(weather['DATE'])

start_date = pd.to_datetime('2018-01-01')
end_date = pd.to_datetime('2018-12-30')

selected_rows = weather[(weather['DATE'] >= start_date) & (weather['DATE'] <= end_date)]

selected_columns = ['TMAX', 'TMIN', 'PRCP','TAVG']
column_means = selected_rows[selected_columns].mean()

print("Column Means:")
print(column_means)

```

    Column Means:
    TMAX    79.100
    TMIN    57.275
    PRCP     9.880
    TAVG    69.500
    dtype: float64
    


```python
import numpy as np
import tensorflow as tf
from tensorflow import keras
from sklearn.model_selection import train_test_split
import pandas as pd

# Assuming you have your 'data' prepared and loaded with the appropriate shape

# Convert 'DATE' column to timestamp format
data['DATE'] = pd.to_datetime(data['DATE'])

# Set random seeds for reproducibility
tf.random.set_seed(42)
np.random.seed(42)

# Specify parameters
history_years = 20  # Number of years for historical data
forecast_year = 1    # Number of years to forecast
num_intervals = 13   # Number of intervals to repeat the process
interval_length = 365  # Length of each interval in days

# Calculate the total length of data
total_years = history_years + forecast_year

# Create an empty list to store forecasting results
forecast_results = []

# Create an empty dictionary to store parameter predictions
parameter_predictions = {
    "PRCP": [],
    "TAVG": [],
    "TMAX": [],
    "TMIN": []
}

# Define the initial start date for the intervals
initial_start_date = pd.Timestamp("1985-01-01")

# Loop over different intervals
for interval in range(num_intervals):
    # Calculate the start and end dates for the historical period
    start_date = initial_start_date + pd.DateOffset(years=interval)
    end_date = start_date + pd.DateOffset(years=history_years)

    # Extract data for the current historical interval
    historical_data = data[(data['DATE'] >= start_date) & (data['DATE'] < end_date)]

    # Calculate the start and end dates for the forecast period
    forecast_start_date = end_date + pd.DateOffset(years=1)  # Add one year for uniform forecasting
    forecast_end_date = forecast_start_date + pd.DateOffset(years=1)

    # Extract data for the current forecast interval
    forecast_data = data[(data['DATE'] >= forecast_start_date) & (data['DATE'] < forecast_end_date)]

    # Split historical data into train and test sets
    train_data, test_data = train_test_split(historical_data, test_size=0.2, shuffle=False)

    # Create Stacked Denoising Autoencoder
    your_input_shape = historical_data.shape[1] - 1
    your_output_shape = your_input_shape  # Define your output shape here

    denoising_encoder = keras.models.Sequential([
        keras.layers.Flatten(input_shape=[your_input_shape]),
        keras.layers.GaussianNoise(0.9),
        keras.layers.Dense(100, activation="selu"),
        keras.layers.Dropout(0.5),  # Adding dropout layer to the encoder
        keras.layers.Dense(30, activation="selu")
    ])

    denoising_decoder = keras.models.Sequential([
        keras.layers.Dense(100, activation="selu", input_shape=[30]),
        keras.layers.Dropout(0.9),  # Adding dropout layer to the decoder
        keras.layers.Dense(your_output_shape, activation="linear"),  # Use linear activation for output layer
        keras.layers.Reshape([your_output_shape])
    ])

    denoising_ae = keras.models.Sequential([denoising_encoder, denoising_decoder])
    denoising_ae.compile(loss="mean_squared_error", optimizer=keras.optimizers.Adam(learning_rate=0.001))

    # Early Stopping callback
    early_stopping = keras.callbacks.EarlyStopping(monitor='val_loss', patience=10)

    # Train the autoencoder on train data with validation loss monitoring
    history = denoising_ae.fit(train_data.drop('DATE', axis=1), train_data.drop('DATE', axis=1),
                               epochs=60, batch_size=32,
                               validation_data=(test_data.drop('DATE', axis=1),
                                                test_data.drop('DATE', axis=1)),
                               callbacks=[early_stopping],
                               verbose=1)

    # Display validation loss for each epoch
    print(f"Validation Loss for Interval {interval + 1}:")
    print(history.history['val_loss'])
    print("=" * 40)

    # Use the trained autoencoder for forecasting
    encoded_forecast = denoising_ae.layers[0](forecast_data.drop('DATE', axis=1).values)  # Access encoder layers
    decoded_forecast = denoising_ae.layers[1](encoded_forecast)  # Access decoder layers

    # Store the decoded forecast results for this interval
    forecast_results.append(decoded_forecast)

    # Display parameter predictions for this interval
    print(f"Decoded Forecasts for Interval {interval + 1} (Forecast Date: {forecast_start_date.date()}):")
    for param_idx, param_name in enumerate(["PRCP", "TAVG", "TMAX", "TMIN"]):
        param_prediction = decoded_forecast[:, param_idx]
        parameter_predictions[param_name].extend(param_prediction)
        avg_param_prediction = np.mean(param_prediction)  # Calculate average prediction
        print(f"{param_name}: {param_prediction} (Average: {avg_param_prediction:.2f})")
    print("=" * 40)

    # Move the initial start date for the next interval
    initial_start_date += pd.DateOffset(years=0)

```

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    Epoch 1/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m5s[0m 109ms/step - loss: 4344.9248 - val_loss: 3049.1267
    Epoch 2/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3834.8745 - val_loss: 2629.0254
    Epoch 3/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 3282.7698 - val_loss: 2375.6252
    Epoch 4/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 2831.4724 - val_loss: 2068.9395
    Epoch 5/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 2670.0857 - val_loss: 1812.6698
    Epoch 6/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 2286.8330 - val_loss: 1620.4141
    Epoch 7/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 2204.1841 - val_loss: 1438.2100
    Epoch 8/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 2111.3660 - val_loss: 1269.8734
    Epoch 9/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 1995.7959 - val_loss: 1173.2228
    Epoch 10/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1863.0463 - val_loss: 1071.4274
    Epoch 11/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1642.6609 - val_loss: 924.0958
    Epoch 12/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1850.6978 - val_loss: 862.1804
    Epoch 13/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1637.6995 - val_loss: 844.9617
    Epoch 14/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 1435.5219 - val_loss: 866.0417
    Epoch 15/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1394.8867 - val_loss: 871.3786
    Epoch 16/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 1451.3396 - val_loss: 799.3826
    Epoch 17/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1294.7802 - val_loss: 674.8914
    Epoch 18/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 1415.2263 - val_loss: 598.0349
    Epoch 19/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 1205.8641 - val_loss: 553.2383
    Epoch 20/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 1177.7144 - val_loss: 528.5812
    Epoch 21/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1146.9725 - val_loss: 532.0892
    Epoch 22/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1224.5764 - val_loss: 483.1042
    Epoch 23/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1251.3241 - val_loss: 493.9369
    Epoch 24/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1030.9927 - val_loss: 528.0586
    Epoch 25/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1027.3076 - val_loss: 537.3908
    Epoch 26/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 986.5048 - val_loss: 503.8214
    Epoch 27/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1011.4991 - val_loss: 510.1512
    Epoch 28/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1025.1034 - val_loss: 513.5243
    Epoch 29/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 1016.3696 - val_loss: 543.9088
    Epoch 30/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1084.0164 - val_loss: 548.8528
    Epoch 31/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 1081.3925 - val_loss: 505.2508
    Epoch 32/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 947.1591 - val_loss: 422.4427
    Epoch 33/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1066.0952 - val_loss: 423.3113
    Epoch 34/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 841.1795 - val_loss: 413.2348
    Epoch 35/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1100.5100 - val_loss: 403.4008
    Epoch 36/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 944.2950 - val_loss: 412.2869
    Epoch 37/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 864.9270 - val_loss: 406.1331
    Epoch 38/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 39ms/step - loss: 917.7071 - val_loss: 382.2775
    Epoch 39/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 853.3477 - val_loss: 318.7069
    Epoch 40/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 847.4503 - val_loss: 327.9843
    Epoch 41/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 850.1159 - val_loss: 369.1075
    Epoch 42/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 857.7132 - val_loss: 404.8621
    Epoch 43/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 765.1096 - val_loss: 377.2565
    Epoch 44/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 844.2972 - val_loss: 322.1647
    Epoch 45/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 908.1061 - val_loss: 307.6328
    Epoch 46/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 779.7493 - val_loss: 292.0583
    Epoch 47/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 834.3438 - val_loss: 252.2493
    Epoch 48/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 756.5740 - val_loss: 224.4516
    Epoch 49/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 712.8189 - val_loss: 263.3007
    Epoch 50/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 649.5798 - val_loss: 282.1568
    Epoch 51/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 703.6179 - val_loss: 310.0684
    Epoch 52/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 774.6760 - val_loss: 323.7483
    Epoch 53/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 661.4733 - val_loss: 308.0930
    Epoch 54/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 595.0797 - val_loss: 273.6583
    Epoch 55/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 680.5947 - val_loss: 222.5908
    Epoch 56/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 611.5627 - val_loss: 175.1922
    Epoch 57/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 643.8862 - val_loss: 165.0235
    Epoch 58/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 691.7428 - val_loss: 181.8103
    Epoch 59/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 596.7184 - val_loss: 241.1523
    Epoch 60/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 672.1356 - val_loss: 296.7453
    Validation Loss for Interval 1:
    [3049.126708984375, 2629.025390625, 2375.625244140625, 2068.939453125, 1812.6697998046875, 1620.4140625, 1438.2099609375, 1269.8734130859375, 1173.2227783203125, 1071.4273681640625, 924.0958251953125, 862.1803588867188, 844.961669921875, 866.041748046875, 871.3786010742188, 799.3826293945312, 674.891357421875, 598.034912109375, 553.2383422851562, 528.5811767578125, 532.0892333984375, 483.10418701171875, 493.9368896484375, 528.05859375, 537.3908081054688, 503.82135009765625, 510.1512145996094, 513.5242919921875, 543.9088134765625, 548.852783203125, 505.2507629394531, 422.4426574707031, 423.311279296875, 413.23480224609375, 403.4007873535156, 412.286865234375, 406.133056640625, 382.2774658203125, 318.7068786621094, 327.9842834472656, 369.1075134277344, 404.862060546875, 377.25653076171875, 322.16473388671875, 307.6328125, 292.05828857421875, 252.24932861328125, 224.45155334472656, 263.3006896972656, 282.1568298339844, 310.0683898925781, 323.7483215332031, 308.0929870605469, 273.6582946777344, 222.5908203125, 175.19219970703125, 165.0235137939453, 181.8103485107422, 241.1522979736328, 296.7452697753906]
    ========================================
    Decoded Forecasts for Interval 1 (Forecast Date: 2006-01-01):
    PRCP: [2.833762  2.8322659 2.769926  2.7803402 2.7297385 2.8265233 2.8299236
     2.8288627] (Average: 2.80)
    TAVG: [50.816036 50.795513 50.151974 49.59077  48.84075  50.889137 51.397705
     51.47165 ] (Average: 50.49)
    TMAX: [57.102463 57.07293  56.018154 55.479027 54.399124 57.147133 57.862946
     57.937393] (Average: 56.63)
    TMIN: [41.78591  41.767754 41.111584 40.681923 40.01258  41.838028 42.22593
     42.281624] (Average: 41.46)
    ========================================
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    Epoch 1/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m5s[0m 111ms/step - loss: 5360.8823 - val_loss: 3727.2437
    Epoch 2/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 4118.6133 - val_loss: 3284.0996
    Epoch 3/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3619.0239 - val_loss: 3033.1082
    Epoch 4/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 3333.6038 - val_loss: 2811.2798
    Epoch 5/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 2903.0986 - val_loss: 2562.3684
    Epoch 6/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2870.0620 - val_loss: 2263.0227
    Epoch 7/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2397.5068 - val_loss: 1906.0536
    Epoch 8/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 2122.2451 - val_loss: 1516.8741
    Epoch 9/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2054.7651 - val_loss: 1165.4650
    Epoch 10/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 1697.7357 - val_loss: 913.7234
    Epoch 11/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1681.0891 - val_loss: 715.9318
    Epoch 12/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1826.6682 - val_loss: 658.6857
    Epoch 13/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1626.5250 - val_loss: 678.0659
    Epoch 14/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 1465.9763 - val_loss: 695.7240
    Epoch 15/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1241.6788 - val_loss: 708.8528
    Epoch 16/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1339.7631 - val_loss: 715.1188
    Epoch 17/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1224.9836 - val_loss: 666.2219
    Epoch 18/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1275.8218 - val_loss: 563.7759
    Epoch 19/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 1206.4694 - val_loss: 504.4029
    Epoch 20/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 31ms/step - loss: 1171.3744 - val_loss: 503.6330
    Epoch 21/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 1040.5392 - val_loss: 533.5630
    Epoch 22/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 1117.6345 - val_loss: 540.9435
    Epoch 23/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1067.2871 - val_loss: 482.0161
    Epoch 24/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 944.1859 - val_loss: 419.9520
    Epoch 25/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1023.3382 - val_loss: 445.7800
    Epoch 26/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1070.1929 - val_loss: 441.5343
    Epoch 27/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 950.5831 - val_loss: 420.5990
    Epoch 28/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 963.0725 - val_loss: 396.7702
    Epoch 29/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 838.8942 - val_loss: 376.7180
    Epoch 30/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1056.1095 - val_loss: 388.6854
    Epoch 31/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 999.6484 - val_loss: 443.3435
    Epoch 32/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1004.2500 - val_loss: 489.9053
    Epoch 33/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 889.0110 - val_loss: 470.2148
    Epoch 34/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 888.0803 - val_loss: 383.4236
    Epoch 35/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 857.0995 - val_loss: 307.8075
    Epoch 36/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 851.1753 - val_loss: 271.7188
    Epoch 37/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 884.1258 - val_loss: 278.0772
    Epoch 38/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 851.3337 - val_loss: 314.9316
    Epoch 39/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 975.9844 - val_loss: 351.7339
    Epoch 40/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 788.2448 - val_loss: 354.2623
    Epoch 41/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 845.1535 - val_loss: 333.2251
    Epoch 42/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 872.1410 - val_loss: 315.0243
    Epoch 43/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 737.3961 - val_loss: 332.1209
    Epoch 44/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 840.5502 - val_loss: 338.7557
    Epoch 45/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 748.5868 - val_loss: 357.3937
    Epoch 46/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 735.0614 - val_loss: 313.3190
    Validation Loss for Interval 2:
    [3727.24365234375, 3284.099609375, 3033.108154296875, 2811.27978515625, 2562.368408203125, 2263.022705078125, 1906.0535888671875, 1516.8741455078125, 1165.4649658203125, 913.723388671875, 715.9318237304688, 658.6857299804688, 678.0658569335938, 695.7239990234375, 708.852783203125, 715.1187744140625, 666.2218627929688, 563.77587890625, 504.4028625488281, 503.6330261230469, 533.5630493164062, 540.9435424804688, 482.01611328125, 419.95196533203125, 445.77996826171875, 441.5342712402344, 420.5989990234375, 396.7701721191406, 376.718017578125, 388.6853942871094, 443.3434753417969, 489.9053039550781, 470.2147521972656, 383.4236145019531, 307.8075256347656, 271.71881103515625, 278.0771789550781, 314.93157958984375, 351.73388671875, 354.2622985839844, 333.22509765625, 315.0242614746094, 332.12091064453125, 338.7557373046875, 357.3936767578125, 313.3190002441406]
    ========================================
    Decoded Forecasts for Interval 2 (Forecast Date: 2007-01-01):
    PRCP: [2.3145173 2.3221173 2.3330665 2.3341048] (Average: 2.33)
    TAVG: [49.483707 49.359005 49.16975  49.405804] (Average: 49.35)
    TMAX: [55.51656  55.40905  55.244827 55.545425] (Average: 55.43)
    TMIN: [41.002056 40.89262  40.724834 40.878666] (Average: 40.87)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m5s[0m 112ms/step - loss: 3669.7778 - val_loss: 2527.2954
    Epoch 2/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 3128.7107 - val_loss: 2131.6323
    Epoch 3/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2607.7014 - val_loss: 1883.8940
    Epoch 4/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 2391.9746 - val_loss: 1630.5468
    Epoch 5/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 2515.0647 - val_loss: 1403.2268
    Epoch 6/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1948.5503 - val_loss: 1160.4919
    Epoch 7/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1940.3890 - val_loss: 1013.9895
    Epoch 8/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1832.7964 - val_loss: 983.9290
    Epoch 9/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 2018.4369 - val_loss: 1029.3967
    Epoch 10/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1609.9542 - val_loss: 1089.0881
    Epoch 11/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1489.5686 - val_loss: 1046.7875
    Epoch 12/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1378.6038 - val_loss: 925.2825
    Epoch 13/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1453.2018 - val_loss: 740.6366
    Epoch 14/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1481.1697 - val_loss: 628.4041
    Epoch 15/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1303.5801 - val_loss: 545.6191
    Epoch 16/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1323.1824 - val_loss: 552.6990
    Epoch 17/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 1233.2076 - val_loss: 551.9090
    Epoch 18/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1154.3970 - val_loss: 541.1669
    Epoch 19/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1117.6162 - val_loss: 543.4055
    Epoch 20/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1189.1932 - val_loss: 576.9146
    Epoch 21/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1118.3689 - val_loss: 654.7177
    Epoch 22/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1110.3503 - val_loss: 668.4470
    Epoch 23/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1044.7528 - val_loss: 597.6774
    Epoch 24/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1045.5968 - val_loss: 488.7798
    Epoch 25/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 894.2895 - val_loss: 432.1837
    Epoch 26/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1003.4713 - val_loss: 425.5319
    Epoch 27/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 939.2833 - val_loss: 406.7414
    Epoch 28/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 1056.8427 - val_loss: 529.2460
    Epoch 29/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 975.0833 - val_loss: 655.1802
    Epoch 30/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 905.9736 - val_loss: 615.7499
    Epoch 31/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 870.4524 - val_loss: 469.9890
    Epoch 32/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 879.0576 - val_loss: 377.3554
    Epoch 33/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 870.5774 - val_loss: 327.6000
    Epoch 34/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 801.7172 - val_loss: 305.3484
    Epoch 35/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 873.1688 - val_loss: 321.7618
    Epoch 36/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 755.2693 - val_loss: 354.1682
    Epoch 37/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 895.5714 - val_loss: 429.5264
    Epoch 38/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 769.0881 - val_loss: 438.3431
    Epoch 39/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 793.3327 - val_loss: 408.7174
    Epoch 40/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 790.6816 - val_loss: 358.1823
    Epoch 41/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 739.3792 - val_loss: 323.3011
    Epoch 42/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 738.8776 - val_loss: 348.1793
    Epoch 43/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 716.4862 - val_loss: 328.1789
    Epoch 44/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 795.9090 - val_loss: 344.4584
    Validation Loss for Interval 3:
    [2527.29541015625, 2131.63232421875, 1883.89404296875, 1630.5467529296875, 1403.226806640625, 1160.491943359375, 1013.989501953125, 983.928955078125, 1029.396728515625, 1089.088134765625, 1046.7874755859375, 925.2825317382812, 740.6365966796875, 628.404052734375, 545.619140625, 552.6990356445312, 551.9089965820312, 541.1668701171875, 543.405517578125, 576.9146118164062, 654.7176513671875, 668.447021484375, 597.6774291992188, 488.77984619140625, 432.1837158203125, 425.53192138671875, 406.7414245605469, 529.2459716796875, 655.1802368164062, 615.7498779296875, 469.9889831542969, 377.3553771972656, 327.5999755859375, 305.3483581542969, 321.7618408203125, 354.168212890625, 429.5263671875, 438.3431396484375, 408.7174377441406, 358.18231201171875, 323.3011474609375, 348.17926025390625, 328.1788635253906, 344.4583740234375]
    ========================================
    Decoded Forecasts for Interval 3 (Forecast Date: 2008-01-01):
    PRCP: [2.609595  2.5688548 2.5726697] (Average: 2.58)
    TAVG: [46.826878 47.62605  47.538486] (Average: 47.33)
    TMAX: [54.282566 55.449875 55.322742] (Average: 55.02)
    TMIN: [38.81128  39.49948  39.425293] (Average: 39.25)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m4s[0m 108ms/step - loss: 3997.9824 - val_loss: 2770.1030
    Epoch 2/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3473.1123 - val_loss: 2330.1870
    Epoch 3/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 2925.2402 - val_loss: 2023.9088
    Epoch 4/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2742.7881 - val_loss: 1779.3138
    Epoch 5/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 2409.8792 - val_loss: 1540.0190
    Epoch 6/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2237.0410 - val_loss: 1342.6023
    Epoch 7/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1919.1703 - val_loss: 1223.7408
    Epoch 8/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1930.9242 - val_loss: 1121.8036
    Epoch 9/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1743.8276 - val_loss: 1031.8369
    Epoch 10/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1832.9573 - val_loss: 1027.1206
    Epoch 11/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1637.5475 - val_loss: 965.1666
    Epoch 12/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1479.3829 - val_loss: 884.8511
    Epoch 13/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1431.4209 - val_loss: 779.5695
    Epoch 14/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1466.2693 - val_loss: 691.7388
    Epoch 15/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1563.9546 - val_loss: 636.6392
    Epoch 16/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 1473.2946 - val_loss: 595.0458
    Epoch 17/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 1211.3751 - val_loss: 573.3423
    Epoch 18/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1289.1851 - val_loss: 562.8097
    Epoch 19/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1226.8928 - val_loss: 521.6694
    Epoch 20/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1113.7366 - val_loss: 475.1173
    Epoch 21/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1063.0906 - val_loss: 435.0221
    Epoch 22/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1138.2737 - val_loss: 458.0092
    Epoch 23/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 983.1959 - val_loss: 482.2415
    Epoch 24/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1023.7173 - val_loss: 425.9910
    Epoch 25/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 1134.8292 - val_loss: 369.7831
    Epoch 26/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 955.4413 - val_loss: 335.9526
    Epoch 27/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1018.8223 - val_loss: 303.8492
    Epoch 28/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 30ms/step - loss: 1032.5450 - val_loss: 296.4972
    Epoch 29/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 974.1422 - val_loss: 287.6284
    Epoch 30/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 888.7673 - val_loss: 311.9690
    Epoch 31/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1031.2662 - val_loss: 309.1424
    Epoch 32/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 984.8002 - val_loss: 319.4900
    Epoch 33/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 850.3038 - val_loss: 314.4576
    Epoch 34/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 903.1664 - val_loss: 311.7341
    Epoch 35/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 819.0338 - val_loss: 327.6902
    Epoch 36/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 860.5614 - val_loss: 315.9322
    Epoch 37/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 876.7206 - val_loss: 308.5956
    Epoch 38/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 804.3661 - val_loss: 337.5101
    Epoch 39/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 766.4313 - val_loss: 366.5485
    Validation Loss for Interval 4:
    [2770.10302734375, 2330.18701171875, 2023.9088134765625, 1779.3138427734375, 1540.01904296875, 1342.602294921875, 1223.7408447265625, 1121.8035888671875, 1031.8369140625, 1027.12060546875, 965.1665649414062, 884.85107421875, 779.5694580078125, 691.7388305664062, 636.63916015625, 595.0458374023438, 573.34228515625, 562.8096923828125, 521.66943359375, 475.1173095703125, 435.0221252441406, 458.0092468261719, 482.241455078125, 425.99102783203125, 369.7831115722656, 335.95257568359375, 303.8492126464844, 296.4971618652344, 287.6283874511719, 311.968994140625, 309.14239501953125, 319.4899597167969, 314.4576416015625, 311.734130859375, 327.69024658203125, 315.9321594238281, 308.5955810546875, 337.5101013183594, 366.5484924316406]
    ========================================
    Decoded Forecasts for Interval 4 (Forecast Date: 2009-01-01):
    PRCP: [1.7890099 1.7898437 1.8255016 1.7302758 1.7313403 1.7363179] (Average: 1.77)
    TAVG: [49.84004  49.884365 48.346275 47.233715 47.265163 47.370136] (Average: 48.32)
    TMAX: [55.116734 55.15997  53.233356 51.98892  52.017296 52.107742] (Average: 53.27)
    TMIN: [38.70989  38.775375 37.595272 36.784462 36.835594 37.01756 ] (Average: 37.62)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m4s[0m 147ms/step - loss: 4699.4316 - val_loss: 3666.9924
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 4129.4531 - val_loss: 3095.3701
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 3526.0566 - val_loss: 2618.9827
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 2668.9280 - val_loss: 2237.9229
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 2540.1968 - val_loss: 1930.1410
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 2471.0605 - val_loss: 1674.6105
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 2381.3945 - val_loss: 1463.8354
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 2225.8823 - val_loss: 1303.0609
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1963.8562 - val_loss: 1130.8556
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1910.5002 - val_loss: 945.5778
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1842.2063 - val_loss: 787.2361
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1546.5461 - val_loss: 689.8835
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1590.8000 - val_loss: 634.4252
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 1709.9012 - val_loss: 637.5850
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1204.0822 - val_loss: 636.6436
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1350.7374 - val_loss: 622.9525
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1216.3209 - val_loss: 583.8659
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 1266.5941 - val_loss: 549.6772
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 1312.8712 - val_loss: 525.1984
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 1147.9357 - val_loss: 533.2883
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 1210.4739 - val_loss: 514.6938
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1164.4474 - val_loss: 475.5763
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1048.7427 - val_loss: 386.0362
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1038.6527 - val_loss: 317.1532
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 944.3809 - val_loss: 304.4685
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 963.0134 - val_loss: 300.8183
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1016.9539 - val_loss: 275.4302
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1046.3573 - val_loss: 280.6852
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 981.8300 - val_loss: 292.5854
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1093.2974 - val_loss: 318.1048
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 839.3497 - val_loss: 347.1638
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1019.1757 - val_loss: 388.5940
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 890.4826 - val_loss: 405.2512
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 886.2728 - val_loss: 362.4162
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 877.1972 - val_loss: 302.0786
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 924.4893 - val_loss: 232.5640
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 824.3810 - val_loss: 242.5863
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 976.4208 - val_loss: 288.4412
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 797.0191 - val_loss: 321.2563
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 806.6882 - val_loss: 311.2809
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 716.3149 - val_loss: 258.1584
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 867.6976 - val_loss: 227.4937
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 724.1135 - val_loss: 241.3889
    Epoch 44/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 887.7507 - val_loss: 274.0821
    Epoch 45/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 728.2252 - val_loss: 279.9427
    Epoch 46/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 881.8553 - val_loss: 263.5074
    Epoch 47/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 887.0793 - val_loss: 314.7299
    Epoch 48/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 874.2319 - val_loss: 319.8907
    Epoch 49/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 818.2783 - val_loss: 281.0757
    Epoch 50/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 754.6422 - val_loss: 256.5480
    Epoch 51/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 919.7112 - val_loss: 233.7390
    Epoch 52/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 708.9932 - val_loss: 176.4925
    Epoch 53/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 615.0970 - val_loss: 140.2223
    Epoch 54/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 724.0295 - val_loss: 147.3503
    Epoch 55/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 665.6985 - val_loss: 174.4928
    Epoch 56/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 749.9852 - val_loss: 234.8643
    Epoch 57/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 603.5476 - val_loss: 272.2573
    Epoch 58/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 760.9066 - val_loss: 250.9015
    Epoch 59/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 664.3438 - val_loss: 198.6195
    Epoch 60/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 608.6842 - val_loss: 140.5268
    Validation Loss for Interval 5:
    [3666.992431640625, 3095.3701171875, 2618.982666015625, 2237.9228515625, 1930.1409912109375, 1674.6104736328125, 1463.83544921875, 1303.0609130859375, 1130.8555908203125, 945.5777587890625, 787.236083984375, 689.8834838867188, 634.4251708984375, 637.5850219726562, 636.6435546875, 622.9525146484375, 583.8659057617188, 549.6771850585938, 525.1983642578125, 533.288330078125, 514.69384765625, 475.5763244628906, 386.03619384765625, 317.1532287597656, 304.468505859375, 300.81829833984375, 275.43017578125, 280.68524169921875, 292.58538818359375, 318.1047668457031, 347.163818359375, 388.5940246582031, 405.2511901855469, 362.4162292480469, 302.0786437988281, 232.56398010253906, 242.58628845214844, 288.4411926269531, 321.25634765625, 311.2808532714844, 258.1583557128906, 227.4937286376953, 241.38893127441406, 274.0820617675781, 279.9426574707031, 263.5074157714844, 314.7298889160156, 319.89068603515625, 281.07574462890625, 256.5479736328125, 233.7389678955078, 176.49252319335938, 140.22230529785156, 147.3502960205078, 174.49278259277344, 234.86428833007812, 272.25732421875, 250.90145874023438, 198.6195068359375, 140.52679443359375]
    ========================================
    Decoded Forecasts for Interval 5 (Forecast Date: 2010-01-01):
    PRCP: [3.664124  3.7749677 3.766195  3.697949 ] (Average: 3.73)
    TAVG: [53.707684 56.269066 56.22204  55.904606] (Average: 55.53)
    TMAX: [63.45611 66.19999 66.11153 65.52388] (Average: 65.32)
    TMIN: [44.699577 46.63804  46.56084  46.033012] (Average: 45.98)
    ========================================
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    Epoch 1/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m4s[0m 124ms/step - loss: 3655.5476 - val_loss: 2289.5645
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 3374.4487 - val_loss: 2115.0698
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 2769.2700 - val_loss: 1954.8250
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 2655.8252 - val_loss: 1842.2263
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 2422.1499 - val_loss: 1722.5570
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 32ms/step - loss: 2434.0781 - val_loss: 1607.3802
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 2050.7549 - val_loss: 1471.0012
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 2115.0044 - val_loss: 1295.5243
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1865.8168 - val_loss: 1101.3174
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1822.0475 - val_loss: 897.5787
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1650.4688 - val_loss: 796.8052
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1759.9872 - val_loss: 702.1933
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1575.3204 - val_loss: 668.2971
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1451.8558 - val_loss: 655.6595
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1582.1307 - val_loss: 618.8483
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1248.7211 - val_loss: 558.2733
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1509.3441 - val_loss: 517.2305
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1363.0273 - val_loss: 447.8970
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1359.8547 - val_loss: 396.8224
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1075.6470 - val_loss: 375.4962
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1088.2356 - val_loss: 351.3648
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1116.4152 - val_loss: 358.7221
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1177.6111 - val_loss: 397.5874
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1109.2913 - val_loss: 408.3086
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 993.7933 - val_loss: 402.8822
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1118.2968 - val_loss: 401.4376
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1014.1013 - val_loss: 382.4413
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1058.0261 - val_loss: 333.4451
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1020.9692 - val_loss: 277.9500
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 918.1537 - val_loss: 244.5494
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 918.5798 - val_loss: 251.7165
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 884.8078 - val_loss: 257.6266
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 857.4285 - val_loss: 279.5644
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 756.6827 - val_loss: 287.7770
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 670.0286 - val_loss: 267.7602
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 870.8807 - val_loss: 262.3873
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 945.2595 - val_loss: 281.9317
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 735.6724 - val_loss: 268.6166
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 790.3767 - val_loss: 228.0039
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 837.2697 - val_loss: 212.7448
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 30ms/step - loss: 776.8394 - val_loss: 216.8465
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 810.7863 - val_loss: 210.2867
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 679.8604 - val_loss: 211.6363
    Epoch 44/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 651.1476 - val_loss: 199.7715
    Epoch 45/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 762.5190 - val_loss: 191.8268
    Epoch 46/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 733.8258 - val_loss: 199.8601
    Epoch 47/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 675.1875 - val_loss: 183.6292
    Epoch 48/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 757.7117 - val_loss: 168.8537
    Epoch 49/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 704.0807 - val_loss: 162.0430
    Epoch 50/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 645.5117 - val_loss: 205.8207
    Epoch 51/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 638.6085 - val_loss: 241.9937
    Epoch 52/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 688.7129 - val_loss: 223.2053
    Epoch 53/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 679.3201 - val_loss: 201.9351
    Epoch 54/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 580.4543 - val_loss: 178.0428
    Epoch 55/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 644.8826 - val_loss: 165.7428
    Epoch 56/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 597.4708 - val_loss: 140.2569
    Epoch 57/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 710.1370 - val_loss: 129.9831
    Epoch 58/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 556.5169 - val_loss: 125.9038
    Epoch 59/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 663.5167 - val_loss: 156.2425
    Epoch 60/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 730.2036 - val_loss: 170.0820
    Validation Loss for Interval 6:
    [2289.564453125, 2115.06982421875, 1954.824951171875, 1842.226318359375, 1722.5570068359375, 1607.3802490234375, 1471.001220703125, 1295.5242919921875, 1101.3173828125, 897.5786743164062, 796.8052368164062, 702.1932983398438, 668.297119140625, 655.6595458984375, 618.8482666015625, 558.2733154296875, 517.23046875, 447.89703369140625, 396.8223571777344, 375.49615478515625, 351.3647766113281, 358.72210693359375, 397.5873718261719, 408.30859375, 402.8822021484375, 401.4375915527344, 382.44134521484375, 333.44512939453125, 277.949951171875, 244.54937744140625, 251.71646118164062, 257.6266174316406, 279.56439208984375, 287.7769775390625, 267.7601623535156, 262.38726806640625, 281.93170166015625, 268.6165771484375, 228.00389099121094, 212.74481201171875, 216.84646606445312, 210.28668212890625, 211.63629150390625, 199.77154541015625, 191.8267822265625, 199.860107421875, 183.62918090820312, 168.85365295410156, 162.04299926757812, 205.8206787109375, 241.9936981201172, 223.2052764892578, 201.93507385253906, 178.04283142089844, 165.74276733398438, 140.25689697265625, 129.98312377929688, 125.90377044677734, 156.24252319335938, 170.08200073242188]
    ========================================
    Decoded Forecasts for Interval 6 (Forecast Date: 2011-01-01):
    PRCP: [3.4739645 3.4561808 3.464409 ] (Average: 3.46)
    TAVG: [54.96312 55.33747 54.90867] (Average: 55.07)
    TMAX: [61.650116 62.18615  61.69371 ] (Average: 61.84)
    TMIN: [46.45517  46.81158  46.393635] (Average: 46.55)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m4s[0m 137ms/step - loss: 6133.1016 - val_loss: 3311.5969
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 4551.7046 - val_loss: 2855.1985
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 3860.7339 - val_loss: 2549.6421
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 3321.9331 - val_loss: 2289.3032
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 2741.9504 - val_loss: 2043.3019
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 2622.3779 - val_loss: 1803.7848
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 2378.7937 - val_loss: 1580.8179
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 2311.0281 - val_loss: 1356.2491
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1996.0032 - val_loss: 1189.6708
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 2151.1699 - val_loss: 1090.9738
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1927.7283 - val_loss: 1029.6274
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1950.0685 - val_loss: 999.1669
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1841.3618 - val_loss: 964.1336
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1631.7552 - val_loss: 937.7112
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1734.4655 - val_loss: 871.9764
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 1518.4589 - val_loss: 836.8245
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1709.0519 - val_loss: 801.8152
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 39ms/step - loss: 1422.1783 - val_loss: 762.2496
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 1646.2570 - val_loss: 736.7849
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 38ms/step - loss: 1382.8186 - val_loss: 752.6442
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1444.3745 - val_loss: 714.9182
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1310.4987 - val_loss: 637.6059
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1297.8840 - val_loss: 564.4065
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 1204.0156 - val_loss: 495.7163
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 1503.4227 - val_loss: 479.2006
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 1299.0084 - val_loss: 536.1674
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 1350.3459 - val_loss: 601.9349
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 1238.7141 - val_loss: 628.2937
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1178.8463 - val_loss: 620.5161
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 1201.6034 - val_loss: 562.8503
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 1142.1764 - val_loss: 490.5406
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1064.3406 - val_loss: 422.0491
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 963.5641 - val_loss: 427.2919
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1079.1024 - val_loss: 408.7739
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1047.4375 - val_loss: 402.0254
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1115.8585 - val_loss: 389.2929
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1058.5288 - val_loss: 382.5127
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 938.1378 - val_loss: 370.0822
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1070.9263 - val_loss: 374.9488
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 915.5802 - val_loss: 400.5711
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 942.0928 - val_loss: 397.0699
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 946.0953 - val_loss: 372.4210
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 883.5005 - val_loss: 373.5121
    Epoch 44/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 798.5872 - val_loss: 361.2281
    Epoch 45/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 953.9548 - val_loss: 347.4042
    Epoch 46/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 914.4714 - val_loss: 368.8719
    Epoch 47/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 812.8909 - val_loss: 375.9636
    Epoch 48/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 980.8335 - val_loss: 380.1441
    Epoch 49/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 30ms/step - loss: 974.4927 - val_loss: 372.5831
    Epoch 50/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 935.6058 - val_loss: 357.1525
    Epoch 51/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 822.0234 - val_loss: 352.4185
    Epoch 52/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 861.7802 - val_loss: 363.3253
    Epoch 53/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 846.4587 - val_loss: 343.7201
    Epoch 54/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 32ms/step - loss: 878.4441 - val_loss: 289.1597
    Epoch 55/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 977.9556 - val_loss: 242.6652
    Epoch 56/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 887.6650 - val_loss: 254.0246
    Epoch 57/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 872.4445 - val_loss: 288.6850
    Epoch 58/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 804.6995 - val_loss: 311.5705
    Epoch 59/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 723.3665 - val_loss: 306.2798
    Epoch 60/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 797.3116 - val_loss: 287.8988
    Validation Loss for Interval 7:
    [3311.596923828125, 2855.198486328125, 2549.64208984375, 2289.30322265625, 2043.3018798828125, 1803.7847900390625, 1580.81787109375, 1356.2491455078125, 1189.6707763671875, 1090.9737548828125, 1029.62744140625, 999.1669311523438, 964.1336059570312, 937.7112426757812, 871.9764404296875, 836.824462890625, 801.815185546875, 762.2496337890625, 736.784912109375, 752.6442260742188, 714.9181518554688, 637.6058959960938, 564.406494140625, 495.7163391113281, 479.20062255859375, 536.1674194335938, 601.9349365234375, 628.293701171875, 620.5160522460938, 562.8502807617188, 490.5406188964844, 422.0491027832031, 427.2918701171875, 408.7738952636719, 402.0254211425781, 389.29290771484375, 382.5126647949219, 370.0822448730469, 374.94879150390625, 400.5711364746094, 397.0699157714844, 372.4210205078125, 373.5120544433594, 361.2280578613281, 347.4041748046875, 368.87188720703125, 375.9635925292969, 380.14410400390625, 372.5831298828125, 357.15252685546875, 352.41851806640625, 363.32525634765625, 343.7200927734375, 289.15966796875, 242.6652374267578, 254.02462768554688, 288.6849670410156, 311.5704650878906, 306.27978515625, 287.8988037109375]
    ========================================
    Decoded Forecasts for Interval 7 (Forecast Date: 2012-01-01):
    PRCP: [1.9964943 1.9983592 1.9910997 2.0006967] (Average: 2.00)
    TAVG: [52.039936 51.6451   52.63296  52.600376] (Average: 52.23)
    TMAX: [55.78258  55.360996 56.417797 56.424915] (Average: 56.00)
    TMIN: [41.122364 40.84704  41.532066 41.526398] (Average: 41.26)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m5s[0m 150ms/step - loss: 5953.8057 - val_loss: 3733.5403
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 4731.2168 - val_loss: 3319.2390
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 3815.6758 - val_loss: 2996.8342
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 3481.3765 - val_loss: 2743.3669
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 3295.2996 - val_loss: 2549.9465
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 3013.1096 - val_loss: 2353.2268
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 2519.8977 - val_loss: 2147.7063
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 2535.9214 - val_loss: 1934.3046
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 2309.4426 - val_loss: 1696.8202
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 2192.8945 - val_loss: 1461.2328
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 2142.3130 - val_loss: 1251.2401
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1946.4752 - val_loss: 1118.1754
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1833.0396 - val_loss: 1036.2029
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 30ms/step - loss: 1814.6266 - val_loss: 1002.7111
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 1576.9274 - val_loss: 983.0279
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1726.5521 - val_loss: 967.0620
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1638.4978 - val_loss: 904.8055
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 1466.3628 - val_loss: 806.6273
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 1563.6815 - val_loss: 721.1569
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1574.2327 - val_loss: 663.7034
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 1596.1293 - val_loss: 655.8203
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1465.8225 - val_loss: 655.3725
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1470.3801 - val_loss: 651.1993
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1298.3422 - val_loss: 653.6576
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 1190.7867 - val_loss: 672.8663
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1244.5146 - val_loss: 669.2255
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1259.3640 - val_loss: 635.4650
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1188.6619 - val_loss: 580.4151
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1217.4105 - val_loss: 569.5965
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1215.5266 - val_loss: 579.5671
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1114.4761 - val_loss: 531.2616
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1125.8057 - val_loss: 468.4909
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 964.5369 - val_loss: 386.0009
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1038.6017 - val_loss: 343.9636
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 31ms/step - loss: 1088.9299 - val_loss: 345.8243
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 939.2549 - val_loss: 374.9265
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 1021.2133 - val_loss: 399.1802
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 951.2291 - val_loss: 445.0741
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 970.2864 - val_loss: 448.3013
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 984.6087 - val_loss: 416.1863
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 957.8759 - val_loss: 383.1592
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 767.4199 - val_loss: 353.6878
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1037.1707 - val_loss: 359.8696
    Epoch 44/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 930.4946 - val_loss: 413.0821
    Validation Loss for Interval 8:
    [3733.540283203125, 3319.239013671875, 2996.834228515625, 2743.366943359375, 2549.946533203125, 2353.226806640625, 2147.706298828125, 1934.3045654296875, 1696.8201904296875, 1461.2327880859375, 1251.2401123046875, 1118.1754150390625, 1036.202880859375, 1002.7111206054688, 983.0278930664062, 967.0619506835938, 904.8054809570312, 806.6272583007812, 721.1569213867188, 663.7034301757812, 655.8202514648438, 655.3724975585938, 651.1992797851562, 653.6575927734375, 672.8663330078125, 669.2255249023438, 635.4649658203125, 580.4151000976562, 569.5964965820312, 579.5670776367188, 531.2615966796875, 468.4909362792969, 386.0008850097656, 343.9635925292969, 345.82427978515625, 374.9264831542969, 399.18023681640625, 445.0741271972656, 448.30133056640625, 416.1863098144531, 383.1591796875, 353.6877746582031, 359.86962890625, 413.0820617675781]
    ========================================
    Decoded Forecasts for Interval 8 (Forecast Date: 2013-01-01):
    PRCP: [4.384357] (Average: 4.38)
    TAVG: [46.930607] (Average: 46.93)
    TMAX: [52.887444] (Average: 52.89)
    TMIN: [36.198742] (Average: 36.20)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m5s[0m 143ms/step - loss: 4341.2583 - val_loss: 2858.4739
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 3589.8899 - val_loss: 2537.2769
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3164.7776 - val_loss: 2268.9150
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 2885.2810 - val_loss: 2034.4197
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 2592.1099 - val_loss: 1781.4430
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 2229.0427 - val_loss: 1511.0720
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 2196.9485 - val_loss: 1248.5125
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 2050.6714 - val_loss: 1034.3954
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 2155.6184 - val_loss: 887.6884
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 36ms/step - loss: 1831.0854 - val_loss: 817.9542
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 1970.6914 - val_loss: 822.8591
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1759.2296 - val_loss: 822.3842
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1688.6195 - val_loss: 819.2477
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1586.4824 - val_loss: 825.7173
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1593.6642 - val_loss: 856.5511
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 1468.1447 - val_loss: 808.4732
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1419.7926 - val_loss: 751.4259
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1720.1628 - val_loss: 776.6560
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1386.3213 - val_loss: 742.0379
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1276.3947 - val_loss: 682.3374
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1312.6278 - val_loss: 640.8081
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 1164.0253 - val_loss: 628.1034
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1321.3295 - val_loss: 620.6976
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1245.1458 - val_loss: 645.4883
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1182.0746 - val_loss: 701.9414
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1330.8534 - val_loss: 740.9615
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1080.6069 - val_loss: 712.6883
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1080.3245 - val_loss: 665.3082
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1118.2721 - val_loss: 600.2437
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1108.7518 - val_loss: 536.8420
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 1040.5854 - val_loss: 454.7354
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 1012.4253 - val_loss: 419.0717
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1044.8325 - val_loss: 396.8713
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 1149.4440 - val_loss: 397.8647
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1025.0134 - val_loss: 408.9428
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1216.0228 - val_loss: 424.8521
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1017.4063 - val_loss: 455.2901
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1011.3135 - val_loss: 462.9030
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1060.5134 - val_loss: 471.2314
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 30ms/step - loss: 930.0444 - val_loss: 445.5493
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 802.6303 - val_loss: 378.5921
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 1125.4034 - val_loss: 328.8021
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1064.0717 - val_loss: 331.6881
    Epoch 44/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 877.6668 - val_loss: 392.1085
    Epoch 45/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 849.2386 - val_loss: 421.8586
    Epoch 46/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 744.6744 - val_loss: 424.4453
    Epoch 47/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 720.1097 - val_loss: 384.7039
    Epoch 48/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 828.8426 - val_loss: 318.4308
    Epoch 49/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 814.4338 - val_loss: 241.7346
    Epoch 50/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 884.8777 - val_loss: 231.4504
    Epoch 51/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 32ms/step - loss: 743.2643 - val_loss: 200.0625
    Epoch 52/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 862.0131 - val_loss: 209.0677
    Epoch 53/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 839.4768 - val_loss: 257.5871
    Epoch 54/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 713.3474 - val_loss: 310.7602
    Epoch 55/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 644.8314 - val_loss: 360.0671
    Epoch 56/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 808.4003 - val_loss: 359.6098
    Epoch 57/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 766.1897 - val_loss: 334.3784
    Epoch 58/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 692.8054 - val_loss: 320.5220
    Epoch 59/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 779.9861 - val_loss: 307.2465
    Epoch 60/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 722.7908 - val_loss: 260.0757
    Validation Loss for Interval 9:
    [2858.473876953125, 2537.27685546875, 2268.9150390625, 2034.419677734375, 1781.4429931640625, 1511.072021484375, 1248.512451171875, 1034.3953857421875, 887.6884155273438, 817.9542236328125, 822.859130859375, 822.3842163085938, 819.2477416992188, 825.71728515625, 856.5510864257812, 808.4732055664062, 751.4259033203125, 776.656005859375, 742.0379028320312, 682.33740234375, 640.80810546875, 628.1033935546875, 620.6976318359375, 645.48828125, 701.94140625, 740.9614868164062, 712.6882934570312, 665.3081665039062, 600.24365234375, 536.842041015625, 454.73541259765625, 419.07171630859375, 396.87127685546875, 397.86468505859375, 408.9427795410156, 424.85211181640625, 455.2900695800781, 462.9029541015625, 471.23138427734375, 445.5493469238281, 378.5921325683594, 328.8021240234375, 331.6880798339844, 392.1085205078125, 421.8586120605469, 424.44525146484375, 384.703857421875, 318.4308166503906, 241.73455810546875, 231.45037841796875, 200.06248474121094, 209.0676727294922, 257.58709716796875, 310.7601623535156, 360.067138671875, 359.6098327636719, 334.37835693359375, 320.52203369140625, 307.2464904785156, 260.0757141113281]
    ========================================
    Decoded Forecasts for Interval 9 (Forecast Date: 2014-01-01):
    PRCP: [2.0067298 2.0360959 2.0660443 2.0688052] (Average: 2.04)
    TAVG: [50.65456  50.400074 50.035275 49.87156 ] (Average: 50.24)
    TMAX: [59.70495  59.43349  59.072075 58.861214] (Average: 59.27)
    TMIN: [43.454155 43.18689  42.83316  42.699696] (Average: 43.04)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m5s[0m 144ms/step - loss: 5017.4761 - val_loss: 3166.5176
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 4029.7515 - val_loss: 2862.4990
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3833.2920 - val_loss: 2621.0889
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 3208.1145 - val_loss: 2382.9661
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 34ms/step - loss: 3035.7454 - val_loss: 2170.5127
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 2667.0105 - val_loss: 1983.2085
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 2466.5249 - val_loss: 1796.4983
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 2459.4790 - val_loss: 1618.5413
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 2430.9250 - val_loss: 1445.7600
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 2123.8789 - val_loss: 1284.0430
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 2060.5349 - val_loss: 1150.6930
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 34ms/step - loss: 2033.8212 - val_loss: 1019.0947
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 2014.2728 - val_loss: 905.9069
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 2032.1735 - val_loss: 815.1566
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 30ms/step - loss: 1954.0660 - val_loss: 757.2710
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1712.6693 - val_loss: 703.2288
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1889.0018 - val_loss: 665.7601
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 1977.6373 - val_loss: 657.0131
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1519.5552 - val_loss: 657.5995
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1666.7633 - val_loss: 655.2971
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1708.3832 - val_loss: 680.4874
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1612.6471 - val_loss: 730.5026
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1370.3966 - val_loss: 832.5187
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1582.1439 - val_loss: 947.9626
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1549.9048 - val_loss: 976.2736
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1529.8975 - val_loss: 907.9822
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1823.9971 - val_loss: 821.6021
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 38ms/step - loss: 1578.5149 - val_loss: 702.5156
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 1365.1006 - val_loss: 604.7352
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1473.6121 - val_loss: 526.6332
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 1377.7723 - val_loss: 477.1361
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 1238.9036 - val_loss: 441.7575
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1394.5233 - val_loss: 436.2474
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 1195.6177 - val_loss: 525.0291
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 36ms/step - loss: 1427.6000 - val_loss: 571.1498
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 1168.6748 - val_loss: 578.8275
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 1428.2122 - val_loss: 575.7633
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 1340.6934 - val_loss: 541.2452
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 35ms/step - loss: 1260.5177 - val_loss: 488.7589
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 48ms/step - loss: 1216.1268 - val_loss: 445.7810
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 1204.5454 - val_loss: 437.4738
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1256.8894 - val_loss: 469.9168
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1148.4843 - val_loss: 461.3313
    Validation Loss for Interval 10:
    [3166.517578125, 2862.4990234375, 2621.0888671875, 2382.966064453125, 2170.5126953125, 1983.20849609375, 1796.498291015625, 1618.541259765625, 1445.760009765625, 1284.04296875, 1150.6929931640625, 1019.0946655273438, 905.9068603515625, 815.1566162109375, 757.27099609375, 703.2288208007812, 665.7601318359375, 657.0130615234375, 657.5995483398438, 655.2970581054688, 680.4873657226562, 730.5025634765625, 832.5186767578125, 947.962646484375, 976.2736206054688, 907.982177734375, 821.60205078125, 702.5155639648438, 604.7352294921875, 526.6331787109375, 477.1361083984375, 441.75750732421875, 436.24737548828125, 525.029052734375, 571.1497802734375, 578.8275146484375, 575.7633056640625, 541.2452392578125, 488.7588806152344, 445.781005859375, 437.4737548828125, 469.91680908203125, 461.3313293457031]
    ========================================
    Decoded Forecasts for Interval 10 (Forecast Date: 2015-01-01):
    PRCP: [2.8640232 2.8667195 2.874766  2.8749032] (Average: 2.87)
    TAVG: [46.566044 46.267555 45.757263 44.677025] (Average: 45.82)
    TMAX: [54.975246 54.73681  54.346508 53.38583 ] (Average: 54.36)
    TMIN: [36.67714  36.50191  36.214947 35.5421  ] (Average: 36.23)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m4s[0m 222ms/step - loss: 4207.9990 - val_loss: 3296.3723
    Epoch 2/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 3717.3108 - val_loss: 2920.1565
    Epoch 3/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 3534.3892 - val_loss: 2612.8154
    Epoch 4/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 30ms/step - loss: 2975.4822 - val_loss: 2327.9392
    Epoch 5/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 2969.1294 - val_loss: 2064.5017
    Epoch 6/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 2564.6919 - val_loss: 1846.4965
    Epoch 7/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 2496.6719 - val_loss: 1630.6394
    Epoch 8/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 2181.8711 - val_loss: 1428.2228
    Epoch 9/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 2370.3440 - val_loss: 1267.7758
    Epoch 10/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 2128.6616 - val_loss: 1132.4669
    Epoch 11/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 1890.7767 - val_loss: 987.1714
    Epoch 12/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 1824.6254 - val_loss: 840.0032
    Epoch 13/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 1736.2026 - val_loss: 750.5621
    Epoch 14/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 1886.6619 - val_loss: 727.7233
    Epoch 15/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 1588.9965 - val_loss: 747.6588
    Epoch 16/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 1673.6266 - val_loss: 800.0455
    Epoch 17/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 1696.1342 - val_loss: 869.1414
    Epoch 18/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 1686.6384 - val_loss: 895.5508
    Epoch 19/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 1555.2834 - val_loss: 890.6272
    Epoch 20/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 1503.8041 - val_loss: 852.5914
    Epoch 21/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 1568.9829 - val_loss: 765.8713
    Epoch 22/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 1524.3604 - val_loss: 652.4857
    Epoch 23/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 1306.6475 - val_loss: 542.4838
    Epoch 24/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 1222.1641 - val_loss: 465.8334
    Epoch 25/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 1303.0021 - val_loss: 434.1467
    Epoch 26/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 1326.2085 - val_loss: 407.3172
    Epoch 27/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 1152.1932 - val_loss: 406.8755
    Epoch 28/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 1144.9718 - val_loss: 416.8482
    Epoch 29/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 1345.2095 - val_loss: 411.0733
    Epoch 30/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 1191.1705 - val_loss: 416.0775
    Epoch 31/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 1231.6639 - val_loss: 443.1318
    Epoch 32/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 1286.4816 - val_loss: 459.3185
    Epoch 33/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 1123.6577 - val_loss: 467.3961
    Epoch 34/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 1101.5720 - val_loss: 456.7182
    Epoch 35/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 1060.7965 - val_loss: 455.6790
    Epoch 36/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 1098.6002 - val_loss: 435.2397
    Epoch 37/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 1168.4038 - val_loss: 394.7831
    Epoch 38/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 950.1102 - val_loss: 369.3766
    Epoch 39/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 858.6940 - val_loss: 337.0342
    Epoch 40/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 918.5861 - val_loss: 321.4006
    Epoch 41/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 963.0524 - val_loss: 306.6295
    Epoch 42/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 956.3572 - val_loss: 291.5493
    Epoch 43/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 994.0825 - val_loss: 276.4882
    Epoch 44/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 798.2051 - val_loss: 260.2596
    Epoch 45/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 997.4048 - val_loss: 285.7502
    Epoch 46/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 955.4579 - val_loss: 330.0498
    Epoch 47/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 885.3257 - val_loss: 334.0644
    Epoch 48/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 885.5917 - val_loss: 310.8974
    Epoch 49/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 993.0455 - val_loss: 304.6008
    Epoch 50/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 1006.6670 - val_loss: 326.3523
    Epoch 51/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 963.9067 - val_loss: 347.3448
    Epoch 52/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 41ms/step - loss: 824.4893 - val_loss: 364.9232
    Epoch 53/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 989.7130 - val_loss: 363.4187
    Epoch 54/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 897.3701 - val_loss: 351.2924
    Validation Loss for Interval 11:
    [3296.372314453125, 2920.156494140625, 2612.8154296875, 2327.939208984375, 2064.501708984375, 1846.4964599609375, 1630.639404296875, 1428.2227783203125, 1267.7757568359375, 1132.4669189453125, 987.17138671875, 840.0032348632812, 750.5621337890625, 727.7232666015625, 747.6588134765625, 800.0455322265625, 869.1414184570312, 895.55078125, 890.627197265625, 852.5913696289062, 765.8712768554688, 652.4856567382812, 542.4838256835938, 465.8334045410156, 434.14666748046875, 407.3171691894531, 406.8755187988281, 416.84820556640625, 411.0732727050781, 416.0774841308594, 443.1318359375, 459.31854248046875, 467.3960876464844, 456.7182312011719, 455.6790466308594, 435.2397155761719, 394.7831115722656, 369.3766174316406, 337.03424072265625, 321.4006042480469, 306.62945556640625, 291.5493469238281, 276.4881591796875, 260.2595520019531, 285.7502136230469, 330.0498046875, 334.0643615722656, 310.8973693847656, 304.600830078125, 326.3523254394531, 347.3447570800781, 364.9232482910156, 363.4187316894531, 351.2924499511719]
    ========================================
    Decoded Forecasts for Interval 11 (Forecast Date: 2016-01-01):
    PRCP: [4.1255045] (Average: 4.13)
    TAVG: [46.267513] (Average: 46.27)
    TMAX: [54.07411] (Average: 54.07)
    TMIN: [40.90006] (Average: 40.90)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m5s[0m 206ms/step - loss: 3990.6641 - val_loss: 3611.1726
    Epoch 2/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 3581.0764 - val_loss: 3242.9861
    Epoch 3/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 3083.8076 - val_loss: 2894.6575
    Epoch 4/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 3060.5901 - val_loss: 2565.6279
    Epoch 5/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 2792.4072 - val_loss: 2264.8406
    Epoch 6/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 31ms/step - loss: 2591.4697 - val_loss: 1990.2946
    Epoch 7/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 2398.5942 - val_loss: 1749.7253
    Epoch 8/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 2353.2646 - val_loss: 1538.0336
    Epoch 9/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 1967.5649 - val_loss: 1326.7944
    Epoch 10/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 1982.1842 - val_loss: 1128.4669
    Epoch 11/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 42ms/step - loss: 1775.1528 - val_loss: 965.7133
    Epoch 12/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 1958.5120 - val_loss: 825.8325
    Epoch 13/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 1805.9335 - val_loss: 701.3724
    Epoch 14/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 1847.0902 - val_loss: 647.3806
    Epoch 15/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 32ms/step - loss: 1526.8086 - val_loss: 608.6682
    Epoch 16/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 1555.3525 - val_loss: 575.2783
    Epoch 17/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 1657.6990 - val_loss: 559.0822
    Epoch 18/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 1364.0719 - val_loss: 557.3311
    Epoch 19/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 1254.1398 - val_loss: 553.9758
    Epoch 20/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 1391.2673 - val_loss: 548.6205
    Epoch 21/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 1618.8989 - val_loss: 556.7665
    Epoch 22/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 1437.5974 - val_loss: 553.1998
    Epoch 23/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 1209.4780 - val_loss: 534.8416
    Epoch 24/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 1295.3940 - val_loss: 514.5227
    Epoch 25/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 1395.6300 - val_loss: 485.3507
    Epoch 26/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 1122.4105 - val_loss: 470.7028
    Epoch 27/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 42ms/step - loss: 1161.4701 - val_loss: 434.5359
    Epoch 28/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 1208.4381 - val_loss: 392.1797
    Epoch 29/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 990.3989 - val_loss: 371.8031
    Epoch 30/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 1076.7859 - val_loss: 378.4463
    Epoch 31/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 1075.7227 - val_loss: 402.1586
    Epoch 32/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 1058.6783 - val_loss: 431.9810
    Epoch 33/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 1175.8280 - val_loss: 440.4917
    Epoch 34/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 39ms/step - loss: 1126.9500 - val_loss: 414.9701
    Epoch 35/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 33ms/step - loss: 1135.4326 - val_loss: 367.8805
    Epoch 36/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 1137.9375 - val_loss: 345.3316
    Epoch 37/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 1126.5397 - val_loss: 358.7574
    Epoch 38/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 885.4543 - val_loss: 366.6423
    Epoch 39/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 909.0438 - val_loss: 374.0496
    Epoch 40/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 1025.5006 - val_loss: 375.5562
    Epoch 41/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 46ms/step - loss: 1050.1659 - val_loss: 354.3863
    Epoch 42/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 1004.4578 - val_loss: 338.8102
    Epoch 43/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 944.3900 - val_loss: 351.8449
    Epoch 44/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 841.1787 - val_loss: 342.6888
    Epoch 45/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 942.0341 - val_loss: 315.3417
    Epoch 46/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 963.7793 - val_loss: 285.8103
    Epoch 47/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 879.2317 - val_loss: 244.5009
    Epoch 48/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 913.6235 - val_loss: 214.9162
    Epoch 49/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 791.8050 - val_loss: 200.1596
    Epoch 50/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 1048.3599 - val_loss: 198.3108
    Epoch 51/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 910.7057 - val_loss: 225.2583
    Epoch 52/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 835.1987 - val_loss: 270.8995
    Epoch 53/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 930.3769 - val_loss: 303.9287
    Epoch 54/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 888.7152 - val_loss: 302.4931
    Epoch 55/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 812.4919 - val_loss: 285.3477
    Epoch 56/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 694.0641 - val_loss: 253.7830
    Epoch 57/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 806.1397 - val_loss: 220.3631
    Epoch 58/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 900.4420 - val_loss: 201.7887
    Epoch 59/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 949.8192 - val_loss: 205.0724
    Epoch 60/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 767.0399 - val_loss: 208.0719
    Validation Loss for Interval 12:
    [3611.172607421875, 3242.986083984375, 2894.657470703125, 2565.6279296875, 2264.840576171875, 1990.2945556640625, 1749.725341796875, 1538.0335693359375, 1326.79443359375, 1128.4669189453125, 965.7133178710938, 825.8324584960938, 701.3724365234375, 647.380615234375, 608.668212890625, 575.2783203125, 559.0822143554688, 557.3310546875, 553.975830078125, 548.6204833984375, 556.7665405273438, 553.1998291015625, 534.841552734375, 514.522705078125, 485.3506774902344, 470.7027587890625, 434.5358581542969, 392.1796875, 371.8031311035156, 378.4463195800781, 402.1585693359375, 431.9810485839844, 440.4916687011719, 414.9700927734375, 367.8804931640625, 345.3316345214844, 358.7574462890625, 366.642333984375, 374.0495910644531, 375.55615234375, 354.3862609863281, 338.8101806640625, 351.8448791503906, 342.6887512207031, 315.3417053222656, 285.8103332519531, 244.50091552734375, 214.91619873046875, 200.1596221923828, 198.31077575683594, 225.25831604003906, 270.8995056152344, 303.9286804199219, 302.4931335449219, 285.34771728515625, 253.78297424316406, 220.3630828857422, 201.78868103027344, 205.07235717773438, 208.07188415527344]
    ========================================
    Decoded Forecasts for Interval 12 (Forecast Date: 2017-01-01):
    PRCP: [3.2207394 3.309302  3.1923757] (Average: 3.24)
    TAVG: [53.001045 54.30642  52.55092 ] (Average: 53.29)
    TMAX: [60.896145 62.459805 60.35732 ] (Average: 61.24)
    TMIN: [44.539124 45.527447 44.200714] (Average: 44.76)
    ========================================
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    Epoch 1/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m4s[0m 212ms/step - loss: 4039.4097 - val_loss: 2955.0576
    Epoch 2/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 40ms/step - loss: 3846.8428 - val_loss: 2739.7341
    Epoch 3/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 40ms/step - loss: 3447.2766 - val_loss: 2583.4414
    Epoch 4/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 37ms/step - loss: 2975.6003 - val_loss: 2442.9739
    Epoch 5/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 46ms/step - loss: 2904.9526 - val_loss: 2316.0461
    Epoch 6/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 39ms/step - loss: 2743.2527 - val_loss: 2220.2581
    Epoch 7/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 37ms/step - loss: 2556.8376 - val_loss: 2097.2129
    Epoch 8/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 38ms/step - loss: 2544.4397 - val_loss: 1947.8717
    Epoch 9/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 39ms/step - loss: 2329.0002 - val_loss: 1785.0193
    Epoch 10/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 37ms/step - loss: 2420.5544 - val_loss: 1607.1870
    Epoch 11/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 39ms/step - loss: 2245.0247 - val_loss: 1441.8970
    Epoch 12/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 39ms/step - loss: 2280.8896 - val_loss: 1309.1287
    Epoch 13/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 36ms/step - loss: 2084.6206 - val_loss: 1202.8088
    Epoch 14/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 37ms/step - loss: 1915.2751 - val_loss: 1120.9561
    Epoch 15/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 38ms/step - loss: 2108.6316 - val_loss: 1065.3682
    Epoch 16/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 39ms/step - loss: 1927.8671 - val_loss: 1052.1608
    Epoch 17/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 36ms/step - loss: 1805.3875 - val_loss: 990.8307
    Epoch 18/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 39ms/step - loss: 1670.2856 - val_loss: 906.0436
    Epoch 19/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 39ms/step - loss: 1610.4811 - val_loss: 825.2164
    Epoch 20/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 39ms/step - loss: 1635.5641 - val_loss: 760.9666
    Epoch 21/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 40ms/step - loss: 1535.9851 - val_loss: 764.9121
    Epoch 22/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 38ms/step - loss: 1471.5192 - val_loss: 806.5366
    Epoch 23/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 37ms/step - loss: 1441.3467 - val_loss: 827.7641
    Epoch 24/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 39ms/step - loss: 1670.8469 - val_loss: 858.7898
    Epoch 25/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 38ms/step - loss: 1572.9785 - val_loss: 858.8998
    Epoch 26/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 36ms/step - loss: 1449.9227 - val_loss: 796.0247
    Epoch 27/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 38ms/step - loss: 1296.3314 - val_loss: 685.5798
    Epoch 28/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 37ms/step - loss: 1443.0715 - val_loss: 579.6079
    Epoch 29/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 36ms/step - loss: 1303.7416 - val_loss: 488.4835
    Epoch 30/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 37ms/step - loss: 1283.3804 - val_loss: 422.8008
    Epoch 31/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 40ms/step - loss: 1415.7961 - val_loss: 400.3678
    Epoch 32/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 38ms/step - loss: 1068.5662 - val_loss: 396.6910
    Epoch 33/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 38ms/step - loss: 1181.6588 - val_loss: 417.8355
    Epoch 34/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 38ms/step - loss: 1413.2837 - val_loss: 471.8241
    Epoch 35/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 36ms/step - loss: 1185.4976 - val_loss: 516.1379
    Epoch 36/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 36ms/step - loss: 1193.0098 - val_loss: 536.3679
    Epoch 37/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 38ms/step - loss: 1155.7546 - val_loss: 523.0800
    Epoch 38/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 37ms/step - loss: 1153.1682 - val_loss: 494.2831
    Epoch 39/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 35ms/step - loss: 1064.3945 - val_loss: 455.9469
    Epoch 40/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 40ms/step - loss: 1291.1061 - val_loss: 411.8939
    Epoch 41/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 37ms/step - loss: 1082.9315 - val_loss: 368.8672
    Epoch 42/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 35ms/step - loss: 1089.2405 - val_loss: 360.3494
    Epoch 43/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 36ms/step - loss: 1002.8903 - val_loss: 358.2676
    Epoch 44/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 37ms/step - loss: 853.6856 - val_loss: 330.2946
    Epoch 45/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 34ms/step - loss: 1037.7124 - val_loss: 297.1526
    Epoch 46/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 37ms/step - loss: 938.6010 - val_loss: 291.1990
    Epoch 47/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 38ms/step - loss: 1156.3361 - val_loss: 283.9840
    Epoch 48/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 35ms/step - loss: 990.1146 - val_loss: 279.8640
    Epoch 49/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 38ms/step - loss: 1037.3901 - val_loss: 292.0452
    Epoch 50/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 36ms/step - loss: 845.9774 - val_loss: 297.3000
    Epoch 51/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 33ms/step - loss: 1137.1182 - val_loss: 318.8328
    Epoch 52/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 35ms/step - loss: 851.8425 - val_loss: 329.1236
    Epoch 53/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 37ms/step - loss: 863.0453 - val_loss: 351.2136
    Epoch 54/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 32ms/step - loss: 973.0095 - val_loss: 373.5737
    Epoch 55/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 33ms/step - loss: 1060.1786 - val_loss: 395.2895
    Epoch 56/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 36ms/step - loss: 907.7390 - val_loss: 380.5871
    Epoch 57/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 34ms/step - loss: 842.7677 - val_loss: 330.3050
    Epoch 58/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 33ms/step - loss: 803.3075 - val_loss: 276.8632
    Epoch 59/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 35ms/step - loss: 876.1804 - val_loss: 259.3761
    Epoch 60/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 36ms/step - loss: 942.0532 - val_loss: 258.4276
    Validation Loss for Interval 13:
    [2955.0576171875, 2739.734130859375, 2583.44140625, 2442.973876953125, 2316.046142578125, 2220.258056640625, 2097.212890625, 1947.8717041015625, 1785.019287109375, 1607.18701171875, 1441.89697265625, 1309.128662109375, 1202.808837890625, 1120.9560546875, 1065.3681640625, 1052.1607666015625, 990.8306884765625, 906.0435791015625, 825.2164306640625, 760.966552734375, 764.912109375, 806.53662109375, 827.7640991210938, 858.789794921875, 858.8997802734375, 796.024658203125, 685.579833984375, 579.60791015625, 488.4834899902344, 422.8008117675781, 400.3678283691406, 396.69097900390625, 417.8354797363281, 471.8241271972656, 516.1378784179688, 536.367919921875, 523.0799560546875, 494.2831115722656, 455.9468994140625, 411.8939208984375, 368.8671569824219, 360.349365234375, 358.26763916015625, 330.29461669921875, 297.152587890625, 291.198974609375, 283.9839782714844, 279.864013671875, 292.045166015625, 297.3000183105469, 318.8327941894531, 329.12359619140625, 351.213623046875, 373.5736999511719, 395.2895202636719, 380.5870666503906, 330.30499267578125, 276.8631896972656, 259.3760986328125, 258.4276428222656]
    ========================================
    Decoded Forecasts for Interval 13 (Forecast Date: 2018-01-01):
    PRCP: [4.3462706 4.388488  4.461343  4.254299 ] (Average: 4.36)
    TAVG: [51.647564 51.898376 52.084244 51.02617 ] (Average: 51.66)
    TMAX: [58.421597 58.670986 58.85144  57.76266 ] (Average: 58.43)
    TMIN: [43.82716  44.052425 44.190556 43.26125 ] (Average: 43.83)
    ========================================
    


```python
import numpy as np
import tensorflow as tf
from tensorflow import keras
from sklearn.model_selection import train_test_split
import pandas as pd

# Assuming you have your 'data' prepared and loaded with the appropriate shape

# Convert 'DATE' column to timestamp format
data['DATE'] = pd.to_datetime(data['DATE'])

# Set random seeds for reproducibility
tf.random.set_seed(42)
np.random.seed(42)

# Specify parameters
history_years = 20  # Number of years for historical data
forecast_year = 1    # Number of years to forecast
num_intervals = 13   # Number of intervals to repeat the process
interval_length = 365  # Length of each interval in days

# Calculate the total length of data
total_years = history_years + forecast_year

# Create an empty list to store forecasting results
forecast_results = []

# Create an empty dictionary to store parameter predictions
parameter_predictions = {
    "PRCP": [],
    "TAVG": [],
    "TMAX": [],
    "TMIN": []
}

# Define the initial start date for the intervals
initial_start_date = pd.Timestamp("1985-01-01")

# Loop over different intervals
for interval in range(num_intervals):
    # Calculate the start and end dates for the historical period
    start_date = initial_start_date + pd.DateOffset(years=interval)
    end_date = start_date + pd.DateOffset(years=history_years)

    # Extract data for the current historical interval
    historical_data = data[(data['DATE'] >= start_date) & (data['DATE'] < end_date)]

    # Calculate the start and end dates for the forecast period
    forecast_start_date = end_date + pd.DateOffset(years=1)  # Add one year for uniform forecasting
    forecast_end_date = forecast_start_date + pd.DateOffset(years=1)

    # Extract data for the current forecast interval
    forecast_data = data[(data['DATE'] >= forecast_start_date) & (data['DATE'] < forecast_end_date)]

    # Split historical data into train and test sets
    train_data, test_data = train_test_split(historical_data, test_size=0.2, shuffle=False)

    # Create Stacked Denoising Autoencoder
    your_input_shape = historical_data.shape[1] - 1
    your_output_shape = your_input_shape  # Define your output shape here

    denoising_encoder = keras.models.Sequential([
        keras.layers.Flatten(input_shape=[your_input_shape]),
        keras.layers.GaussianNoise(0.2),
        keras.layers.Dense(100, activation="selu"),
        keras.layers.Dense(30, activation="selu")
    ])

    denoising_decoder = keras.models.Sequential([
        keras.layers.Dense(100, activation="selu", input_shape=[30]),
        keras.layers.Dense(your_output_shape, activation="linear"),  # Use linear activation for output layer
        keras.layers.Reshape([your_output_shape])
    ])

    denoising_ae = keras.models.Sequential([denoising_encoder, denoising_decoder])
    denoising_ae.compile(loss="mean_squared_error", optimizer=keras.optimizers.Adam(learning_rate=0.001))

    # Early Stopping callback
    early_stopping = keras.callbacks.EarlyStopping(monitor='val_loss', patience=10)

    # Train the autoencoder on train data with validation loss monitoring
    history = denoising_ae.fit(train_data.drop('DATE', axis=1), train_data.drop('DATE', axis=1),
                               epochs=60, batch_size=32,
                               validation_data=(test_data.drop('DATE', axis=1),
                                                test_data.drop('DATE', axis=1)),
                               callbacks=[early_stopping],
                               verbose=1)

    # Display validation loss for each epoch
    print(f"Validation Loss for Interval {interval + 1}:")
    print(history.history['val_loss'])
    print("=" * 40)

    # Use the trained autoencoder for forecasting
    encoded_forecast = denoising_ae.layers[0](forecast_data.drop('DATE', axis=1).values)  # Access encoder layers
    decoded_forecast = denoising_ae.layers[1](encoded_forecast)  # Access decoder layers

    # Store the decoded forecast results for this interval
    forecast_results.append(decoded_forecast)

    # Display parameter predictions for this interval
    print(f"Decoded Forecasts for Interval {interval + 1} (Forecast Date: {forecast_start_date.date()}):")
    for param_idx, param_name in enumerate(["PRCP", "TAVG", "TMAX", "TMIN"]):
        param_prediction = decoded_forecast[:, param_idx]
        parameter_predictions[param_name].extend(param_prediction)
        avg_param_prediction = np.mean(param_prediction)  # Calculate average prediction
        print(f"{param_name}: {param_prediction} (Average: {avg_param_prediction:.2f})")
    print("=" * 40)

    # Move the initial start date for the next interval
    initial_start_date += pd.DateOffset(years=0)

```

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    Epoch 1/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m5s[0m 133ms/step - loss: 3232.3853 - val_loss: 2742.8499
    Epoch 2/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 2462.3486 - val_loss: 2062.9934
    Epoch 3/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1812.5137 - val_loss: 1361.2079
    Epoch 4/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1143.4147 - val_loss: 683.8907
    Epoch 5/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 529.2295 - val_loss: 181.2631
    Epoch 6/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 116.9668 - val_loss: 22.2156
    Epoch 7/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 32.9668 - val_loss: 105.6338
    Epoch 8/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 102.8450 - val_loss: 94.0207
    Epoch 9/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 71.3551 - val_loss: 28.5809
    Epoch 10/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 18.9823 - val_loss: 13.7647
    Epoch 11/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 12.8328 - val_loss: 20.1565
    Epoch 12/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 18.1711 - val_loss: 18.9503
    Epoch 13/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 15.0486 - val_loss: 13.1070
    Epoch 14/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 9.4901 - val_loss: 10.3043
    Epoch 15/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 7.7298 - val_loss: 10.6863
    Epoch 16/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 8.1245 - val_loss: 10.5899
    Epoch 17/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 7.7567 - val_loss: 9.3840
    Epoch 18/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.9384 - val_loss: 8.9198
    Epoch 19/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 6.7821 - val_loss: 9.2766
    Epoch 20/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.9377 - val_loss: 9.3742
    Epoch 21/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 6.8472 - val_loss: 9.1860
    Epoch 22/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.6968 - val_loss: 9.0831
    Epoch 23/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.6637 - val_loss: 8.9948
    Epoch 24/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.6106 - val_loss: 8.9124
    Epoch 25/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.5711 - val_loss: 8.9453
    Epoch 26/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.5517 - val_loss: 8.9985
    Epoch 27/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 6.5300 - val_loss: 8.9626
    Epoch 28/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.4615 - val_loss: 8.8941
    Epoch 29/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 6.3785 - val_loss: 8.8491
    Epoch 30/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 6.3074 - val_loss: 8.7605
    Epoch 31/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 6.2362 - val_loss: 8.7228
    Epoch 32/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.1666 - val_loss: 8.7460
    Epoch 33/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 6.1336 - val_loss: 8.6543
    Epoch 34/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.0502 - val_loss: 8.6139
    Epoch 35/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 5.9680 - val_loss: 8.5696
    Epoch 36/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 5.8395 - val_loss: 8.6487
    Epoch 37/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 5.7960 - val_loss: 8.3824
    Epoch 38/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 5.6678 - val_loss: 8.0348
    Epoch 39/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.5549 - val_loss: 8.1449
    Epoch 40/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 5.5129 - val_loss: 8.1978
    Epoch 41/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 5.4317 - val_loss: 7.9841
    Epoch 42/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 5.3257 - val_loss: 7.8555
    Epoch 43/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 5.2233 - val_loss: 7.8291
    Epoch 44/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 5.1325 - val_loss: 7.7397
    Epoch 45/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 5.0367 - val_loss: 7.5835
    Epoch 46/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 4.9153 - val_loss: 7.4646
    Epoch 47/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 4.7881 - val_loss: 7.3543
    Epoch 48/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 4.6397 - val_loss: 7.2131
    Epoch 49/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 4.4994 - val_loss: 7.0596
    Epoch 50/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 4.3519 - val_loss: 6.9026
    Epoch 51/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 4.2063 - val_loss: 6.6992
    Epoch 52/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 4.0743 - val_loss: 6.6049
    Epoch 53/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.8976 - val_loss: 6.4200
    Epoch 54/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 3.7587 - val_loss: 6.1939
    Epoch 55/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 3.6084 - val_loss: 6.0316
    Epoch 56/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 3.4731 - val_loss: 5.9255
    Epoch 57/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 3.3580 - val_loss: 5.7657
    Epoch 58/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 3.2394 - val_loss: 5.5779
    Epoch 59/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 3.1460 - val_loss: 5.4935
    Epoch 60/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 3.0675 - val_loss: 5.3702
    Validation Loss for Interval 1:
    [2742.849853515625, 2062.993408203125, 1361.2078857421875, 683.8907470703125, 181.26309204101562, 22.215585708618164, 105.6338119506836, 94.0206527709961, 28.580886840820312, 13.764737129211426, 20.156450271606445, 18.95032501220703, 13.107043266296387, 10.30430793762207, 10.686349868774414, 10.589868545532227, 9.383992195129395, 8.919775009155273, 9.276633262634277, 9.374167442321777, 9.185986518859863, 9.083137512207031, 8.994813919067383, 8.912406921386719, 8.945319175720215, 8.99853229522705, 8.962639808654785, 8.894076347351074, 8.849113464355469, 8.76047134399414, 8.7228422164917, 8.746044158935547, 8.654261589050293, 8.613887786865234, 8.569579124450684, 8.648707389831543, 8.382399559020996, 8.034812927246094, 8.14486026763916, 8.197833061218262, 7.984081745147705, 7.855534553527832, 7.829122543334961, 7.739651203155518, 7.5835041999816895, 7.464595794677734, 7.3543381690979, 7.213077068328857, 7.059612274169922, 6.902584075927734, 6.699155330657959, 6.604895114898682, 6.420027256011963, 6.193888187408447, 6.0315985679626465, 5.925474643707275, 5.7657470703125, 5.5778632164001465, 5.493536949157715, 5.37019681930542]
    ========================================
    Decoded Forecasts for Interval 1 (Forecast Date: 2006-01-01):
    PRCP: [4.6360846 4.630783  4.0334854 4.271867  4.083212  4.564307  8.064956
     8.003723 ] (Average: 5.29)
    TAVG: [68.99404  68.968346 67.554855 66.52219  65.59717  69.16862  68.829445
     68.91367 ] (Average: 68.07)
    TMAX: [81.132935 81.09001  79.023285 78.03456  76.52415  81.24415  81.50493
     81.58453 ] (Average: 80.02)
    TMIN: [56.56821  56.549103 55.595272 54.73891  54.067448 56.7153   56.136974
     56.21496 ] (Average: 55.82)
    ========================================
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    Epoch 1/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m5s[0m 151ms/step - loss: 2358.6201 - val_loss: 1546.4895
    Epoch 2/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1248.9298 - val_loss: 668.8204
    Epoch 3/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 470.5454 - val_loss: 143.9305
    Epoch 4/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 81.3178 - val_loss: 73.3826
    Epoch 5/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 77.7579 - val_loss: 83.9029
    Epoch 6/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 37ms/step - loss: 83.1034 - val_loss: 34.1759
    Epoch 7/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 42.5614 - val_loss: 32.3236
    Epoch 8/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 31.1908 - val_loss: 15.1415
    Epoch 9/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 10.6083 - val_loss: 13.5788
    Epoch 10/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 9.3432 - val_loss: 18.4110
    Epoch 11/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 11.7031 - val_loss: 12.6943
    Epoch 12/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 7.1928 - val_loss: 8.7781
    Epoch 13/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.9238 - val_loss: 8.0080
    Epoch 14/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 6.1811 - val_loss: 6.7547
    Epoch 15/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 5.7946 - val_loss: 6.0864
    Epoch 16/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 5.4579 - val_loss: 6.2382
    Epoch 17/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 5.1216 - val_loss: 7.0480
    Epoch 18/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 4.9366 - val_loss: 7.4746
    Epoch 19/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 4.8543 - val_loss: 6.9535
    Epoch 20/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.7341 - val_loss: 6.3887
    Epoch 21/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.7313 - val_loss: 6.1761
    Epoch 22/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 4.6807 - val_loss: 6.2160
    Epoch 23/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 4.6333 - val_loss: 6.2813
    Epoch 24/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 4.5697 - val_loss: 6.2871
    Epoch 25/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 4.5038 - val_loss: 6.2418
    Validation Loss for Interval 2:
    [1546.489501953125, 668.8204345703125, 143.93045043945312, 73.38263702392578, 83.90290832519531, 34.1758918762207, 32.32363510131836, 15.141549110412598, 13.578775405883789, 18.411006927490234, 12.694311141967773, 8.778077125549316, 8.008003234863281, 6.754726409912109, 6.086399078369141, 6.238150596618652, 7.048020839691162, 7.474592208862305, 6.953537464141846, 6.388681888580322, 6.17612361907959, 6.216015815734863, 6.281299591064453, 6.287055492401123, 6.241750240325928]
    ========================================
    Decoded Forecasts for Interval 2 (Forecast Date: 2007-01-01):
    PRCP: [5.0278745 4.951532  4.8357635 4.8298907] (Average: 4.91)
    TAVG: [66.83644 66.6831  66.45238 66.98334] (Average: 66.74)
    TMAX: [79.36171  79.088646 78.68003  79.46082 ] (Average: 79.15)
    TMIN: [56.552532 56.3214   55.974827 56.417023] (Average: 56.32)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m4s[0m 107ms/step - loss: 3128.8032 - val_loss: 2591.1223
    Epoch 2/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 2336.4973 - val_loss: 1890.6450
    Epoch 3/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1674.3654 - val_loss: 1197.0129
    Epoch 4/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 1021.5970 - val_loss: 564.5751
    Epoch 5/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 453.1337 - val_loss: 142.0922
    Epoch 6/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 104.4184 - val_loss: 25.6103
    Epoch 7/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 31.6531 - val_loss: 86.2321
    Epoch 8/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 75.7936 - val_loss: 83.4670
    Epoch 9/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 61.0883 - val_loss: 35.3264
    Epoch 10/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 23.8462 - val_loss: 12.1642
    Epoch 11/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 11.4278 - val_loss: 10.5470
    Epoch 12/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 13.2020 - val_loss: 10.7428
    Epoch 13/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 13.1369 - val_loss: 9.6089
    Epoch 14/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 10.5295 - val_loss: 8.9021
    Epoch 15/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 8.1856 - val_loss: 9.2073
    Epoch 16/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 7.5586 - val_loss: 9.5549
    Epoch 17/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 7.6454 - val_loss: 8.4097
    Epoch 18/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 7.2850 - val_loss: 7.2687
    Epoch 19/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 6.8822 - val_loss: 6.8994
    Epoch 20/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.8435 - val_loss: 7.1568
    Epoch 21/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.7987 - val_loss: 7.4009
    Epoch 22/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.6846 - val_loss: 7.5450
    Epoch 23/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.5431 - val_loss: 7.5251
    Epoch 24/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 6.4318 - val_loss: 7.2915
    Epoch 25/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.3352 - val_loss: 7.0817
    Epoch 26/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 6.2422 - val_loss: 6.9632
    Epoch 27/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.1491 - val_loss: 6.9296
    Epoch 28/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.0485 - val_loss: 6.9022
    Epoch 29/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 5.9367 - val_loss: 6.8006
    Epoch 30/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 5.7937 - val_loss: 6.6826
    Epoch 31/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 5.6547 - val_loss: 6.5440
    Epoch 32/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.5293 - val_loss: 6.4359
    Epoch 33/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 5.3875 - val_loss: 6.3442
    Epoch 34/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 5.1990 - val_loss: 6.1840
    Epoch 35/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 5.0403 - val_loss: 5.9179
    Epoch 36/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 31ms/step - loss: 4.8490 - val_loss: 5.6175
    Epoch 37/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.6741 - val_loss: 5.5539
    Epoch 38/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 4.5553 - val_loss: 5.4981
    Epoch 39/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 4.4268 - val_loss: 5.4197
    Epoch 40/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.3360 - val_loss: 5.2891
    Epoch 41/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 4.2076 - val_loss: 5.1567
    Epoch 42/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 4.1007 - val_loss: 5.0086
    Epoch 43/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.9725 - val_loss: 4.8993
    Epoch 44/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 3.8710 - val_loss: 4.8087
    Epoch 45/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.7556 - val_loss: 4.7861
    Epoch 46/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 3.6742 - val_loss: 4.6169
    Epoch 47/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 3.5626 - val_loss: 4.4798
    Epoch 48/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 3.4476 - val_loss: 3.8068
    Epoch 49/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 3.2765 - val_loss: 4.0137
    Epoch 50/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.1774 - val_loss: 4.2207
    Epoch 51/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.0852 - val_loss: 3.7903
    Epoch 52/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 2.9851 - val_loss: 3.8318
    Epoch 53/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2.9396 - val_loss: 3.7196
    Epoch 54/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2.8552 - val_loss: 3.6972
    Epoch 55/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 2.7904 - val_loss: 3.5427
    Epoch 56/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 2.7421 - val_loss: 3.4643
    Epoch 57/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2.6662 - val_loss: 3.3937
    Epoch 58/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 2.6125 - val_loss: 3.3178
    Epoch 59/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 2.5725 - val_loss: 3.2383
    Epoch 60/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2.5133 - val_loss: 3.1811
    Validation Loss for Interval 3:
    [2591.122314453125, 1890.64501953125, 1197.012939453125, 564.5751342773438, 142.0921630859375, 25.61028480529785, 86.2320556640625, 83.46701049804688, 35.32643127441406, 12.164229393005371, 10.546967506408691, 10.742791175842285, 9.608855247497559, 8.902135848999023, 9.207265853881836, 9.554889678955078, 8.40968132019043, 7.26869535446167, 6.899387359619141, 7.156772136688232, 7.400930404663086, 7.545045852661133, 7.525089740753174, 7.291473388671875, 7.081745147705078, 6.963155269622803, 6.929580211639404, 6.9021897315979, 6.800589084625244, 6.682611465454102, 6.544034957885742, 6.435857772827148, 6.344210147857666, 6.184025764465332, 5.917882919311523, 5.617460250854492, 5.553884506225586, 5.498088359832764, 5.419734477996826, 5.2891106605529785, 5.156699180603027, 5.008623123168945, 4.899274826049805, 4.80868673324585, 4.786121845245361, 4.616919040679932, 4.479794502258301, 3.8068177700042725, 4.013718128204346, 4.220745086669922, 3.790295124053955, 3.8317761421203613, 3.7195913791656494, 3.69720721244812, 3.542707681655884, 3.464334487915039, 3.3936679363250732, 3.317802667617798, 3.2383012771606445, 3.1811327934265137]
    ========================================
    Decoded Forecasts for Interval 3 (Forecast Date: 2008-01-01):
    PRCP: [9.536392 9.315165 9.338653] (Average: 9.40)
    TAVG: [68.118835 68.941765 68.85426 ] (Average: 68.64)
    TMAX: [79.16242 80.03613 79.94268] (Average: 79.71)
    TMIN: [54.851337 55.796345 55.695362] (Average: 55.45)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m5s[0m 112ms/step - loss: 3619.5620 - val_loss: 2964.1079
    Epoch 2/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 2652.0938 - val_loss: 2202.6978
    Epoch 3/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 1973.0454 - val_loss: 1587.4167
    Epoch 4/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1379.6035 - val_loss: 954.4902
    Epoch 5/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 786.5319 - val_loss: 412.3734
    Epoch 6/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 312.9460 - val_loss: 102.9583
    Epoch 7/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 32ms/step - loss: 78.7555 - val_loss: 42.9845
    Epoch 8/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 53.2373 - val_loss: 65.0392
    Epoch 9/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 65.7985 - val_loss: 52.8291
    Epoch 10/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 42.7830 - val_loss: 32.3530
    Epoch 11/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 22.4551 - val_loss: 20.6702
    Epoch 12/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 14.8144 - val_loss: 12.3973
    Epoch 13/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 11.7517 - val_loss: 9.0993
    Epoch 14/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 11.3251 - val_loss: 9.9746
    Epoch 15/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 11.2752 - val_loss: 10.2423
    Epoch 16/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 9.5975 - val_loss: 9.4211
    Epoch 17/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 8.3418 - val_loss: 9.1104
    Epoch 18/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 8.3829 - val_loss: 8.8037
    Epoch 19/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 8.3293 - val_loss: 8.4489
    Epoch 20/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 8.0390 - val_loss: 8.5003
    Epoch 21/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 8.0632 - val_loss: 8.4568
    Epoch 22/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 8.0725 - val_loss: 7.7308
    Epoch 23/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 7.8484 - val_loss: 7.7829
    Epoch 24/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 7.7716 - val_loss: 8.5925
    Epoch 25/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 7.7692 - val_loss: 8.2172
    Epoch 26/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 7.7202 - val_loss: 7.8443
    Epoch 27/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 7.6743 - val_loss: 7.9999
    Epoch 28/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 7.6378 - val_loss: 7.9178
    Epoch 29/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 7.6056 - val_loss: 7.9113
    Epoch 30/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 7.5747 - val_loss: 7.9438
    Epoch 31/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 7.5509 - val_loss: 7.8136
    Epoch 32/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 7.5222 - val_loss: 7.8112
    Validation Loss for Interval 4:
    [2964.10791015625, 2202.69775390625, 1587.416748046875, 954.490234375, 412.37335205078125, 102.95832061767578, 42.984458923339844, 65.03924560546875, 52.829139709472656, 32.35304260253906, 20.670238494873047, 12.397346496582031, 9.09926986694336, 9.974618911743164, 10.242345809936523, 9.421124458312988, 9.110411643981934, 8.803672790527344, 8.448923110961914, 8.50033187866211, 8.456753730773926, 7.730784893035889, 7.782937526702881, 8.592506408691406, 8.217208862304688, 7.844266891479492, 7.999876976013184, 7.9177703857421875, 7.911253929138184, 7.943835258483887, 7.8135833740234375, 7.811183929443359]
    ========================================
    Decoded Forecasts for Interval 4 (Forecast Date: 2009-01-01):
    PRCP: [2.971499  2.9999251 3.208551  3.1222024 3.1478639 3.24166  ] (Average: 3.12)
    TAVG: [69.73259  69.92964  67.48165  65.643036 65.80311  66.37188 ] (Average: 67.49)
    TMAX: [80.65235  80.991585 78.49294  75.861725 76.14237  77.1903  ] (Average: 78.22)
    TMIN: [57.095005 57.399403 56.22257  53.96729  54.222454 55.155735] (Average: 55.68)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m5s[0m 140ms/step - loss: 3017.1606 - val_loss: 2462.8743
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 2199.7239 - val_loss: 1765.4176
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1538.3319 - val_loss: 1087.9065
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 904.9401 - val_loss: 503.2878
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 380.9422 - val_loss: 121.2399
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 73.4246 - val_loss: 42.4031
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 46.4471 - val_loss: 128.4699
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 118.0614 - val_loss: 111.8901
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 87.1421 - val_loss: 30.5349
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 23.3836 - val_loss: 5.0904
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 12.0052 - val_loss: 21.4784
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 25.1791 - val_loss: 26.3227
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 23.0953 - val_loss: 15.2014
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 11.1636 - val_loss: 8.0081
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 6.5800 - val_loss: 9.6278
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 43ms/step - loss: 8.9685 - val_loss: 10.8844
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 31ms/step - loss: 9.1600 - val_loss: 9.0797
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 6.7250 - val_loss: 8.0957
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 5.9084 - val_loss: 7.9364
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 6.3633 - val_loss: 7.1418
    Validation Loss for Interval 5:
    [2462.874267578125, 1765.4176025390625, 1087.906494140625, 503.2877502441406, 121.23991394042969, 42.40313720703125, 128.4699249267578, 111.89010620117188, 30.534929275512695, 5.090421199798584, 21.478431701660156, 26.322677612304688, 15.201410293579102, 8.008129119873047, 9.627848625183105, 10.884439468383789, 9.079699516296387, 8.095687866210938, 7.936421871185303, 7.141793251037598]
    ========================================
    Decoded Forecasts for Interval 5 (Forecast Date: 2010-01-01):
    PRCP: [4.254999  4.7462497 4.748292  4.7777214] (Average: 4.63)
    TAVG: [66.07762 70.58902 70.54446 70.26478] (Average: 69.37)
    TMAX: [75.98081 81.00175 80.90679 80.23826] (Average: 79.53)
    TMIN: [53.933167 57.378616 57.337772 57.069725] (Average: 56.43)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m4s[0m 126ms/step - loss: 3533.7705 - val_loss: 2786.2239
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 2445.2056 - val_loss: 1876.9110
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1593.2733 - val_loss: 1066.3090
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 851.4937 - val_loss: 427.8928
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 299.2729 - val_loss: 95.3592
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 31ms/step - loss: 61.4853 - val_loss: 82.0168
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 88.0118 - val_loss: 130.6890
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 121.4629 - val_loss: 76.9052
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 67.5429 - val_loss: 23.1313
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 26.9273 - val_loss: 19.8516
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 25.1138 - val_loss: 26.5507
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 24.7681 - val_loss: 22.1270
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 15.7007 - val_loss: 16.9761
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 10.0988 - val_loss: 17.5297
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 10.9250 - val_loss: 16.2300
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 10.4284 - val_loss: 10.6488
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 7.2822 - val_loss: 7.0096
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 6.1154 - val_loss: 6.9030
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 6.7647 - val_loss: 7.3453
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 6.5744 - val_loss: 7.5727
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.8192 - val_loss: 8.1501
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 5.5394 - val_loss: 8.5273
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.6994 - val_loss: 8.1909
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.6338 - val_loss: 7.6615
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.4235 - val_loss: 7.4035
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.3121 - val_loss: 7.2716
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.1656 - val_loss: 7.1679
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.0725 - val_loss: 7.2653
    Validation Loss for Interval 6:
    [2786.223876953125, 1876.9110107421875, 1066.3089599609375, 427.89276123046875, 95.35917663574219, 82.01675415039062, 130.68896484375, 76.90519714355469, 23.13125228881836, 19.851606369018555, 26.550661087036133, 22.126998901367188, 16.976062774658203, 17.5296630859375, 16.23003387451172, 10.648839950561523, 7.009615898132324, 6.903018474578857, 7.345290184020996, 7.5727219581604, 8.15011978149414, 8.527281761169434, 8.190876007080078, 7.6614532470703125, 7.403481960296631, 7.271627426147461, 7.167943000793457, 7.265255928039551]
    ========================================
    Decoded Forecasts for Interval 6 (Forecast Date: 2011-01-01):
    PRCP: [4.6415596 4.487237  4.252252 ] (Average: 4.46)
    TAVG: [69.691025 70.432014 69.78536 ] (Average: 69.97)
    TMAX: [81.54241 82.33949 81.43998] (Average: 81.77)
    TMIN: [56.82931  57.499775 57.184666] (Average: 57.17)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m4s[0m 158ms/step - loss: 3482.8496 - val_loss: 3187.1155
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 2971.4795 - val_loss: 2732.9124
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 40ms/step - loss: 2541.6587 - val_loss: 2306.0391
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 2118.9478 - val_loss: 1822.4415
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 1633.4773 - val_loss: 1272.8250
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 1094.9093 - val_loss: 704.8602
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 564.5472 - val_loss: 229.3252
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 160.1203 - val_loss: 11.6039
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 18.8287 - val_loss: 81.7369
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 36ms/step - loss: 98.2455 - val_loss: 146.9722
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 124.1887 - val_loss: 76.6572
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 52.9361 - val_loss: 18.2892
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 11.9788 - val_loss: 16.0957
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 16.0495 - val_loss: 26.3912
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 24.2841 - val_loss: 23.4396
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 20.0120 - val_loss: 12.9779
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 11.2653 - val_loss: 7.6718
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 7.6274 - val_loss: 9.2292
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 8.5750 - val_loss: 11.1773
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 8.7857 - val_loss: 10.5746
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 7.5715 - val_loss: 9.2923
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 6.5998 - val_loss: 8.6307
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 6.4893 - val_loss: 8.0480
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 6.5186 - val_loss: 7.4685
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 6.3448 - val_loss: 7.1017
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 6.1455 - val_loss: 7.1463
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 6.0559 - val_loss: 7.3485
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 5.9758 - val_loss: 7.2672
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 5.8256 - val_loss: 7.0378
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 5.7480 - val_loss: 6.9191
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 5.6949 - val_loss: 6.8811
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 5.6328 - val_loss: 6.6798
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 5.5761 - val_loss: 6.4627
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 5.5315 - val_loss: 6.4754
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 5.4594 - val_loss: 6.5454
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 5.3655 - val_loss: 6.1107
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 5.2417 - val_loss: 5.9786
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 5.0453 - val_loss: 5.8541
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 4.9845 - val_loss: 5.2996
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 4.8832 - val_loss: 5.4334
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 4.7132 - val_loss: 5.5811
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 4.5838 - val_loss: 5.0336
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 4.5223 - val_loss: 4.8054
    Epoch 44/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 4.4000 - val_loss: 4.6964
    Epoch 45/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 4.2625 - val_loss: 4.4857
    Epoch 46/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 4.1417 - val_loss: 4.3743
    Epoch 47/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 4.0183 - val_loss: 4.1339
    Epoch 48/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 3.9254 - val_loss: 3.9832
    Epoch 49/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 3.8313 - val_loss: 3.8590
    Epoch 50/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.7208 - val_loss: 3.6883
    Epoch 51/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 3.6115 - val_loss: 3.4657
    Epoch 52/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.5116 - val_loss: 3.2400
    Epoch 53/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.3887 - val_loss: 3.1819
    Epoch 54/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.2242 - val_loss: 2.9881
    Epoch 55/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 3.0677 - val_loss: 2.8017
    Epoch 56/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 30ms/step - loss: 2.9473 - val_loss: 2.6977
    Epoch 57/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 2.9031 - val_loss: 2.4921
    Epoch 58/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 2.7887 - val_loss: 2.4236
    Epoch 59/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 2.7293 - val_loss: 2.2889
    Epoch 60/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 2.6253 - val_loss: 2.1901
    Validation Loss for Interval 7:
    [3187.115478515625, 2732.912353515625, 2306.0390625, 1822.4415283203125, 1272.824951171875, 704.8602294921875, 229.32518005371094, 11.603938102722168, 81.73686218261719, 146.9722442626953, 76.6572036743164, 18.289220809936523, 16.095712661743164, 26.391246795654297, 23.43963623046875, 12.977864265441895, 7.671755790710449, 9.229156494140625, 11.177312850952148, 10.574609756469727, 9.292264938354492, 8.630678176879883, 8.048046112060547, 7.468547344207764, 7.101659297943115, 7.146324157714844, 7.3484907150268555, 7.267234802246094, 7.037769794464111, 6.919050216674805, 6.881137371063232, 6.67982816696167, 6.462705612182617, 6.475350856781006, 6.545372009277344, 6.110671520233154, 5.978575229644775, 5.854072093963623, 5.29958963394165, 5.4334001541137695, 5.581132888793945, 5.03357458114624, 4.805371284484863, 4.69635009765625, 4.4856719970703125, 4.374258518218994, 4.133880138397217, 3.98315167427063, 3.8590281009674072, 3.6882872581481934, 3.4657232761383057, 3.239952564239502, 3.181919574737549, 2.988114595413208, 2.8017187118530273, 2.6977343559265137, 2.4921305179595947, 2.4235804080963135, 2.2889251708984375, 2.19010066986084]
    ========================================
    Decoded Forecasts for Interval 7 (Forecast Date: 2012-01-01):
    PRCP: [9.053212 9.055217 9.052593 9.181644] (Average: 9.09)
    TAVG: [69.94852 69.64962 70.43607 70.29153] (Average: 70.08)
    TMAX: [78.55001 77.83624 79.64517 79.46531] (Average: 78.87)
    TMIN: [56.28117  56.061287 56.604794 56.39003 ] (Average: 56.33)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m4s[0m 152ms/step - loss: 2956.5576 - val_loss: 2283.5002
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 2047.8192 - val_loss: 1483.5521
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 1300.6377 - val_loss: 775.2105
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 653.1444 - val_loss: 264.5346
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 223.8612 - val_loss: 42.6589
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 72.5329 - val_loss: 59.9219
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 91.4949 - val_loss: 79.6746
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 77.8589 - val_loss: 61.8753
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 41.3969 - val_loss: 62.0451
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 33.3933 - val_loss: 58.1991
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 28.8111 - val_loss: 35.3491
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 16.6247 - val_loss: 13.8430
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 10.0905 - val_loss: 4.8967
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 10.2728 - val_loss: 2.8908
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 9.5770 - val_loss: 4.4297
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 32ms/step - loss: 7.8264 - val_loss: 8.9093
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 7.4223 - val_loss: 12.1516
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 7.0656 - val_loss: 11.8072
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 6.1130 - val_loss: 10.1731
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 5.8131 - val_loss: 9.1658
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 6.0187 - val_loss: 8.7454
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 5.8874 - val_loss: 8.8477
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 5.6591 - val_loss: 9.1548
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 5.6334 - val_loss: 8.9539
    Validation Loss for Interval 8:
    [2283.500244140625, 1483.5521240234375, 775.2105102539062, 264.5345764160156, 42.65888595581055, 59.9218635559082, 79.67460632324219, 61.87530517578125, 62.04510498046875, 58.199066162109375, 35.34912872314453, 13.843031883239746, 4.896742820739746, 2.890819787979126, 4.429720878601074, 8.909250259399414, 12.151629447937012, 11.807205200195312, 10.173125267028809, 9.165755271911621, 8.745377540588379, 8.847696304321289, 9.154783248901367, 8.953885078430176]
    ========================================
    Decoded Forecasts for Interval 8 (Forecast Date: 2013-01-01):
    PRCP: [4.1453767] (Average: 4.15)
    TAVG: [67.747375] (Average: 67.75)
    TMAX: [79.383766] (Average: 79.38)
    TMIN: [56.445774] (Average: 56.45)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m4s[0m 138ms/step - loss: 3339.3777 - val_loss: 2962.9827
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 2733.6646 - val_loss: 2300.0684
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 2087.4260 - val_loss: 1551.1438
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1359.7507 - val_loss: 802.3193
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 655.0216 - val_loss: 217.2728
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 145.8874 - val_loss: 21.2892
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 31.8155 - val_loss: 166.6449
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 166.0568 - val_loss: 184.9679
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 143.4143 - val_loss: 68.3597
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 39.0404 - val_loss: 16.6885
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 9.5828 - val_loss: 25.4943
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 26.1237 - val_loss: 32.8919
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 30.8593 - val_loss: 22.7187
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 17.4317 - val_loss: 12.2658
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 6.3367 - val_loss: 12.1499
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 30ms/step - loss: 6.9138 - val_loss: 15.8421
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 9.6876 - val_loss: 15.1043
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 7.7829 - val_loss: 10.2902
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 4.9433 - val_loss: 8.9065
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 4.7946 - val_loss: 9.2288
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 5.1429 - val_loss: 9.6731
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 4.7475 - val_loss: 8.7231
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 4.2832 - val_loss: 8.2705
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 4.3090 - val_loss: 8.8297
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 4.3650 - val_loss: 8.5441
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 4.1001 - val_loss: 7.8806
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 4.0135 - val_loss: 8.7510
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 4.0530 - val_loss: 7.6685
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 3.9397 - val_loss: 7.3598
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 3.8781 - val_loss: 8.0927
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 3.9225 - val_loss: 7.7883
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.8759 - val_loss: 7.7216
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.8719 - val_loss: 7.7176
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 3.8288 - val_loss: 7.3100
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 3.7692 - val_loss: 7.4825
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.7774 - val_loss: 7.5076
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 3.7360 - val_loss: 7.2170
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.7059 - val_loss: 7.2912
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 3.6781 - val_loss: 7.1740
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 3.6611 - val_loss: 7.0608
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 3.6331 - val_loss: 7.0594
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.6157 - val_loss: 6.9685
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 3.5900 - val_loss: 6.8341
    Epoch 44/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 3.5814 - val_loss: 6.7848
    Epoch 45/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 3.5245 - val_loss: 6.7451
    Epoch 46/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 3.5196 - val_loss: 6.5979
    Epoch 47/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 34ms/step - loss: 3.4982 - val_loss: 6.5728
    Epoch 48/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 3.4528 - val_loss: 6.4775
    Epoch 49/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.4459 - val_loss: 6.2975
    Epoch 50/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.3978 - val_loss: 6.3426
    Epoch 51/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 3.3778 - val_loss: 6.2368
    Epoch 52/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 31ms/step - loss: 3.3570 - val_loss: 6.0624
    Epoch 53/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 3.3284 - val_loss: 6.1460
    Epoch 54/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 3.3011 - val_loss: 6.0047
    Epoch 55/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.2652 - val_loss: 5.8654
    Epoch 56/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.2046 - val_loss: 5.8619
    Epoch 57/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.1486 - val_loss: 5.6227
    Epoch 58/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.0853 - val_loss: 5.4102
    Epoch 59/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 3.0418 - val_loss: 5.5859
    Epoch 60/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.0412 - val_loss: 5.3526
    Validation Loss for Interval 9:
    [2962.982666015625, 2300.068359375, 1551.143798828125, 802.3192749023438, 217.2727508544922, 21.289169311523438, 166.64491271972656, 184.9678955078125, 68.35965728759766, 16.688467025756836, 25.49430274963379, 32.89193344116211, 22.718690872192383, 12.265788078308105, 12.149870872497559, 15.842071533203125, 15.104287147521973, 10.290205955505371, 8.906525611877441, 9.228849411010742, 9.673111915588379, 8.723115921020508, 8.27048110961914, 8.829731941223145, 8.544139862060547, 7.880643367767334, 8.751036643981934, 7.668498992919922, 7.35984992980957, 8.092721939086914, 7.788272380828857, 7.721638202667236, 7.717632293701172, 7.310047626495361, 7.48253059387207, 7.507578372955322, 7.217008113861084, 7.291177749633789, 7.1739888191223145, 7.060846328735352, 7.059433937072754, 6.968523025512695, 6.83406925201416, 6.78482723236084, 6.745122909545898, 6.597945213317871, 6.572834491729736, 6.477458953857422, 6.29752254486084, 6.342555999755859, 6.236772537231445, 6.06241512298584, 6.145975112915039, 6.00468111038208, 5.865421772003174, 5.8619160652160645, 5.622662544250488, 5.41022253036499, 5.585887908935547, 5.352551460266113]
    ========================================
    Decoded Forecasts for Interval 9 (Forecast Date: 2014-01-01):
    PRCP: [5.972236  5.7594485 5.521011  5.5697074] (Average: 5.71)
    TAVG: [69.37747 68.86244 68.18092 68.08183] (Average: 68.63)
    TMAX: [81.0557  80.50231 79.7722  79.41125] (Average: 80.19)
    TMIN: [59.524437 58.623146 57.490513 57.359047] (Average: 58.25)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m4s[0m 151ms/step - loss: 4104.2563 - val_loss: 3106.1846
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 2868.9524 - val_loss: 2130.7859
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1920.3679 - val_loss: 1294.6597
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 1117.3094 - val_loss: 619.5728
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 503.8193 - val_loss: 227.1266
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 172.0976 - val_loss: 116.2122
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 98.0139 - val_loss: 97.8016
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 93.1761 - val_loss: 72.4835
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 73.6297 - val_loss: 57.1096
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 53.6703 - val_loss: 49.2157
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 41.7109 - val_loss: 36.7513
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 27.3262 - val_loss: 22.5414
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 12.7008 - val_loss: 18.2165
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 8.5904 - val_loss: 22.1221
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 12.4730 - val_loss: 21.6449
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 12.5326 - val_loss: 16.2042
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 8.0439 - val_loss: 13.6740
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 5.8895 - val_loss: 14.2917
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 6.5686 - val_loss: 13.8304
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 6.8146 - val_loss: 12.5835
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 6.2440 - val_loss: 12.4085
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.9192 - val_loss: 12.6941
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.8701 - val_loss: 12.6130
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 5.7119 - val_loss: 12.7268
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 5.6129 - val_loss: 13.0082
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 5.6002 - val_loss: 12.9220
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 5.5282 - val_loss: 12.2841
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 5.4616 - val_loss: 12.0006
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 5.4749 - val_loss: 12.1878
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 5.5048 - val_loss: 12.1305
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.4583 - val_loss: 11.9951
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 5.4343 - val_loss: 12.1233
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 5.3907 - val_loss: 12.1233
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.3726 - val_loss: 11.9413
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 5.3709 - val_loss: 11.8234
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 5.3567 - val_loss: 11.7856
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.3287 - val_loss: 11.7137
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.3175 - val_loss: 11.5686
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 5.2914 - val_loss: 11.5978
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 5.2642 - val_loss: 11.5922
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.2797 - val_loss: 11.5018
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.2264 - val_loss: 11.4407
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.2129 - val_loss: 11.3878
    Epoch 44/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 5.2060 - val_loss: 11.3439
    Epoch 45/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 5.1821 - val_loss: 11.2717
    Epoch 46/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.1576 - val_loss: 11.1532
    Epoch 47/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 5.1378 - val_loss: 11.1138
    Epoch 48/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.1118 - val_loss: 11.1307
    Epoch 49/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.1127 - val_loss: 10.9840
    Epoch 50/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 5.0985 - val_loss: 10.9399
    Epoch 51/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 5.0784 - val_loss: 10.8761
    Epoch 52/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 5.0437 - val_loss: 10.8174
    Epoch 53/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.0349 - val_loss: 10.8172
    Epoch 54/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 5.0214 - val_loss: 10.7326
    Epoch 55/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 4.9862 - val_loss: 10.5992
    Epoch 56/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 4.9698 - val_loss: 10.6098
    Epoch 57/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 31ms/step - loss: 4.9558 - val_loss: 10.5789
    Epoch 58/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 4.9530 - val_loss: 10.4442
    Epoch 59/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 4.9301 - val_loss: 10.4463
    Epoch 60/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 4.8931 - val_loss: 10.4053
    Validation Loss for Interval 10:
    [3106.1845703125, 2130.785888671875, 1294.65966796875, 619.57275390625, 227.12655639648438, 116.21223449707031, 97.80162811279297, 72.48348236083984, 57.10955047607422, 49.215702056884766, 36.751319885253906, 22.541370391845703, 18.216520309448242, 22.122081756591797, 21.644886016845703, 16.20416831970215, 13.67395305633545, 14.291667938232422, 13.830351829528809, 12.583536148071289, 12.40850830078125, 12.694079399108887, 12.612970352172852, 12.72679328918457, 13.008247375488281, 12.922019958496094, 12.28414535522461, 12.000566482543945, 12.187779426574707, 12.130498886108398, 11.99511432647705, 12.123281478881836, 12.123281478881836, 11.941272735595703, 11.823378562927246, 11.78557014465332, 11.713733673095703, 11.56863021850586, 11.597830772399902, 11.59221076965332, 11.501818656921387, 11.440656661987305, 11.387805938720703, 11.34388542175293, 11.271666526794434, 11.15315055847168, 11.113757133483887, 11.130712509155273, 10.983983993530273, 10.939902305603027, 10.876072883605957, 10.817355155944824, 10.817195892333984, 10.732641220092773, 10.5991792678833, 10.609785079956055, 10.578937530517578, 10.444157600402832, 10.446331977844238, 10.40532112121582]
    ========================================
    Decoded Forecasts for Interval 10 (Forecast Date: 2015-01-01):
    PRCP: [4.316331  4.2386084 4.1470394 3.9655373] (Average: 4.17)
    TAVG: [71.95747  71.53137  70.911446 69.373665] (Average: 70.94)
    TMAX: [83.103004 82.4396   81.345055 79.14312 ] (Average: 81.51)
    TMIN: [59.29035  58.954872 58.575294 57.4369  ] (Average: 58.56)
    ========================================
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    Epoch 1/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m5s[0m 236ms/step - loss: 3652.1401 - val_loss: 3202.2290
    Epoch 2/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 3065.7214 - val_loss: 2802.5598
    Epoch 3/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 2673.7793 - val_loss: 2391.1921
    Epoch 4/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 40ms/step - loss: 2253.5464 - val_loss: 1922.8134
    Epoch 5/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 44ms/step - loss: 1787.4203 - val_loss: 1437.3007
    Epoch 6/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 44ms/step - loss: 1307.1813 - val_loss: 950.0714
    Epoch 7/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 42ms/step - loss: 832.6372 - val_loss: 499.1707
    Epoch 8/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 35ms/step - loss: 410.9945 - val_loss: 163.8082
    Epoch 9/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 119.2394 - val_loss: 18.7020
    Epoch 10/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 20.3905 - val_loss: 65.0454
    Epoch 11/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 83.1827 - val_loss: 154.3707
    Epoch 12/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 152.4748 - val_loss: 148.3777
    Epoch 13/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 127.7332 - val_loss: 76.8262
    Epoch 14/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 57.1123 - val_loss: 23.7074
    Epoch 15/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 14.0916 - val_loss: 12.5675
    Epoch 16/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 43ms/step - loss: 9.9345 - val_loss: 22.4776
    Epoch 17/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 21.6327 - val_loss: 30.8967
    Epoch 18/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 28.7523 - val_loss: 29.2686
    Epoch 19/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 25.1337 - val_loss: 20.6216
    Epoch 20/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 15.7705 - val_loss: 12.4525
    Epoch 21/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 7.8482 - val_loss: 9.5571
    Epoch 22/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 5.6042 - val_loss: 10.9107
    Epoch 23/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 7.2588 - val_loss: 12.2387
    Epoch 24/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 30ms/step - loss: 8.6528 - val_loss: 11.1646
    Epoch 25/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 7.7317 - val_loss: 8.9435
    Epoch 26/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 5.8356 - val_loss: 7.7994
    Epoch 27/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.8762 - val_loss: 8.2350
    Epoch 28/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 51ms/step - loss: 5.1231 - val_loss: 9.1278
    Epoch 29/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 39ms/step - loss: 5.5978 - val_loss: 9.3732
    Epoch 30/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 32ms/step - loss: 5.6346 - val_loss: 8.8515
    Epoch 31/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 33ms/step - loss: 5.2508 - val_loss: 8.1418
    Epoch 32/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 34ms/step - loss: 4.8768 - val_loss: 7.7612
    Epoch 33/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 33ms/step - loss: 4.7791 - val_loss: 7.7698
    Epoch 34/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 31ms/step - loss: 4.8171 - val_loss: 7.9367
    Epoch 35/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.8223 - val_loss: 8.0500
    Epoch 36/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 4.7538 - val_loss: 8.0512
    Epoch 37/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.7031 - val_loss: 7.9716
    Epoch 38/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.6896 - val_loss: 7.8523
    Epoch 39/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 4.7143 - val_loss: 7.7365
    Epoch 40/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 47ms/step - loss: 4.6883 - val_loss: 7.6789
    Epoch 41/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 32ms/step - loss: 4.6288 - val_loss: 7.6818
    Epoch 42/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.6087 - val_loss: 7.7005
    Epoch 43/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 4.5877 - val_loss: 7.6898
    Epoch 44/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 4.5820 - val_loss: 7.6395
    Epoch 45/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 4.5501 - val_loss: 7.5705
    Epoch 46/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 39ms/step - loss: 4.5203 - val_loss: 7.5067
    Epoch 47/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 4.5192 - val_loss: 7.4677
    Epoch 48/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 4.4937 - val_loss: 7.4501
    Epoch 49/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 4.4728 - val_loss: 7.4444
    Epoch 50/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 4.4636 - val_loss: 7.4253
    Epoch 51/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 52ms/step - loss: 4.4457 - val_loss: 7.3828
    Epoch 52/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 43ms/step - loss: 4.4392 - val_loss: 7.3253
    Epoch 53/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 4.3827 - val_loss: 7.2671
    Epoch 54/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 4.3849 - val_loss: 7.2264
    Epoch 55/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 4.3530 - val_loss: 7.2064
    Epoch 56/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.3355 - val_loss: 7.1844
    Epoch 57/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 4.3086 - val_loss: 7.1407
    Epoch 58/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 4.2931 - val_loss: 7.0844
    Epoch 59/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.2737 - val_loss: 7.0169
    Epoch 60/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.2420 - val_loss: 6.9615
    Validation Loss for Interval 11:
    [3202.22900390625, 2802.559814453125, 2391.192138671875, 1922.8133544921875, 1437.3006591796875, 950.0713500976562, 499.170654296875, 163.80819702148438, 18.7020320892334, 65.04542541503906, 154.3706512451172, 148.3777313232422, 76.82624053955078, 23.707422256469727, 12.56747055053711, 22.47764778137207, 30.896686553955078, 29.268583297729492, 20.621623992919922, 12.45251750946045, 9.557064056396484, 10.910674095153809, 12.238655090332031, 11.164597511291504, 8.943521499633789, 7.799434661865234, 8.234989166259766, 9.127778053283691, 9.373163223266602, 8.851476669311523, 8.14176082611084, 7.76119327545166, 7.769809722900391, 7.936691761016846, 8.050028800964355, 8.051159858703613, 7.971642017364502, 7.8523030281066895, 7.7365312576293945, 7.678887367248535, 7.681774616241455, 7.700504302978516, 7.689802646636963, 7.63947057723999, 7.57047176361084, 7.50671911239624, 7.467660427093506, 7.450119495391846, 7.444353103637695, 7.4253435134887695, 7.382750034332275, 7.325322151184082, 7.267088413238525, 7.226376533508301, 7.206363677978516, 7.184370040893555, 7.14072322845459, 7.0844316482543945, 7.016918182373047, 6.961466312408447]
    ========================================
    Decoded Forecasts for Interval 11 (Forecast Date: 2016-01-01):
    PRCP: [5.374704] (Average: 5.37)
    TAVG: [68.7579] (Average: 68.76)
    TMAX: [78.488945] (Average: 78.49)
    TMIN: [57.479008] (Average: 57.48)
    ========================================
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    Epoch 1/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m6s[0m 210ms/step - loss: 2568.9209 - val_loss: 2195.5518
    Epoch 2/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 2054.5625 - val_loss: 1675.4188
    Epoch 3/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 1549.4122 - val_loss: 1166.7737
    Epoch 4/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 1058.1774 - val_loss: 708.8180
    Epoch 5/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 620.8043 - val_loss: 347.9901
    Epoch 6/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 285.5024 - val_loss: 129.5627
    Epoch 7/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 97.4652 - val_loss: 74.9018
    Epoch 8/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 63.8814 - val_loss: 100.7417
    Epoch 9/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 92.2144 - val_loss: 104.0821
    Epoch 10/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 91.9879 - val_loss: 66.7266
    Epoch 11/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 58.7525 - val_loss: 34.3841
    Epoch 12/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 33.0969 - val_loss: 25.4228
    Epoch 13/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 27.1131 - val_loss: 27.8271
    Epoch 14/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 28.3831 - val_loss: 25.9358
    Epoch 15/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 24.5408 - val_loss: 17.5390
    Epoch 16/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 15.2748 - val_loss: 9.7252
    Epoch 17/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 7.7365 - val_loss: 8.4932
    Epoch 18/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 6.9899 - val_loss: 11.3377
    Epoch 19/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 9.7061 - val_loss: 12.3392
    Epoch 20/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 10.5687 - val_loss: 10.0353
    Epoch 21/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 8.5669 - val_loss: 7.4573
    Epoch 22/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 6.4566 - val_loss: 6.7923
    Epoch 23/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 5.9132 - val_loss: 7.3000
    Epoch 24/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 6.2181 - val_loss: 7.4277
    Epoch 25/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 6.2655 - val_loss: 6.8566
    Epoch 26/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 5.9167 - val_loss: 6.2405
    Epoch 27/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 31ms/step - loss: 5.7041 - val_loss: 5.9896
    Epoch 28/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 38ms/step - loss: 5.6441 - val_loss: 6.0167
    Epoch 29/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 5.5827 - val_loss: 6.1621
    Epoch 30/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 5.4552 - val_loss: 6.2370
    Epoch 31/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 31ms/step - loss: 5.3651 - val_loss: 6.1674
    Epoch 32/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 5.3363 - val_loss: 6.0036
    Epoch 33/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 5.3236 - val_loss: 5.9038
    Epoch 34/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 5.2731 - val_loss: 5.9000
    Epoch 35/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 5.2071 - val_loss: 5.9320
    Epoch 36/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 5.1530 - val_loss: 5.8620
    Epoch 37/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 5.1546 - val_loss: 5.6809
    Epoch 38/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 40ms/step - loss: 5.1435 - val_loss: 5.5205
    Epoch 39/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 5.1221 - val_loss: 5.5157
    Epoch 40/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 5.0918 - val_loss: 5.6236
    Epoch 41/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 5.0485 - val_loss: 5.6757
    Epoch 42/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 5.0067 - val_loss: 5.5840
    Epoch 43/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 4.9814 - val_loss: 5.4165
    Epoch 44/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 4.9431 - val_loss: 5.3089
    Epoch 45/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 49ms/step - loss: 4.9373 - val_loss: 5.3171
    Epoch 46/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 4.8875 - val_loss: 5.3512
    Epoch 47/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.8540 - val_loss: 5.3210
    Epoch 48/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 4.8520 - val_loss: 5.2190
    Epoch 49/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 4.8091 - val_loss: 5.1022
    Epoch 50/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 4.7312 - val_loss: 4.9953
    Epoch 51/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.6733 - val_loss: 4.8528
    Epoch 52/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 4.6275 - val_loss: 4.6968
    Epoch 53/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.5803 - val_loss: 4.6217
    Epoch 54/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.5651 - val_loss: 4.6217
    Epoch 55/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 4.5355 - val_loss: 4.6182
    Epoch 56/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 4.4738 - val_loss: 4.5569
    Epoch 57/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.4466 - val_loss: 4.4722
    Epoch 58/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 38ms/step - loss: 4.3449 - val_loss: 4.3793
    Epoch 59/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.2819 - val_loss: 4.2499
    Epoch 60/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.2583 - val_loss: 4.0927
    Validation Loss for Interval 12:
    [2195.5517578125, 1675.4188232421875, 1166.773681640625, 708.8179931640625, 347.9901123046875, 129.5626983642578, 74.90182495117188, 100.7416763305664, 104.08209991455078, 66.72657775878906, 34.384132385253906, 25.42279052734375, 27.82707405090332, 25.935789108276367, 17.539039611816406, 9.725192070007324, 8.493237495422363, 11.337689399719238, 12.339173316955566, 10.035311698913574, 7.457310676574707, 6.792346000671387, 7.299989223480225, 7.427679538726807, 6.8565673828125, 6.2405009269714355, 5.98956298828125, 6.016732692718506, 6.162118911743164, 6.237037181854248, 6.1673903465271, 6.003594875335693, 5.9038496017456055, 5.899971008300781, 5.93198823928833, 5.861995220184326, 5.6808552742004395, 5.5204925537109375, 5.515665054321289, 5.623590469360352, 5.6756510734558105, 5.583992958068848, 5.416514873504639, 5.30886697769165, 5.317050457000732, 5.351202011108398, 5.3210296630859375, 5.219021797180176, 5.102203845977783, 4.995331287384033, 4.852792739868164, 4.696761608123779, 4.621723651885986, 4.621712684631348, 4.618167400360107, 4.5568623542785645, 4.472163200378418, 4.379348278045654, 4.249879837036133, 4.092650890350342]
    ========================================
    Decoded Forecasts for Interval 12 (Forecast Date: 2017-01-01):
    PRCP: [7.03148   7.2141657 6.970664 ] (Average: 7.07)
    TAVG: [69.88142 70.47022 69.68346] (Average: 70.01)
    TMAX: [79.45028 79.89619 79.29592] (Average: 79.55)
    TMIN: [57.13471  58.27239  56.742664] (Average: 57.38)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m4s[0m 212ms/step - loss: 3188.5095 - val_loss: 2608.0444
    Epoch 2/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 2407.9575 - val_loss: 1924.6578
    Epoch 3/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 31ms/step - loss: 1775.4653 - val_loss: 1363.2723
    Epoch 4/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 33ms/step - loss: 1247.1046 - val_loss: 862.7099
    Epoch 5/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 772.7913 - val_loss: 439.7363
    Epoch 6/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 380.0284 - val_loss: 144.0351
    Epoch 7/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 118.5244 - val_loss: 23.2345
    Epoch 8/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 25.2294 - val_loss: 61.8714
    Epoch 9/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 67.4445 - val_loss: 136.8895
    Epoch 10/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 126.7936 - val_loss: 139.9999
    Epoch 11/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 118.5630 - val_loss: 83.0225
    Epoch 12/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 31ms/step - loss: 65.1078 - val_loss: 29.1375
    Epoch 13/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 21.8558 - val_loss: 8.8962
    Epoch 14/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 9.4200 - val_loss: 13.0735
    Epoch 15/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 16.0203 - val_loss: 21.3828
    Epoch 16/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 23.5658 - val_loss: 22.2929
    Epoch 17/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 23.5908 - val_loss: 16.0303
    Epoch 18/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 16.7717 - val_loss: 8.6600
    Epoch 19/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 9.5389 - val_loss: 5.7011
    Epoch 20/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 53ms/step - loss: 6.3733 - val_loss: 7.0251
    Epoch 21/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 34ms/step - loss: 7.1211 - val_loss: 8.8365
    Epoch 22/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 8.5446 - val_loss: 8.6622
    Epoch 23/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 8.4058 - val_loss: 7.5134
    Epoch 24/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 52ms/step - loss: 7.1738 - val_loss: 6.4580
    Epoch 25/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 33ms/step - loss: 6.0160 - val_loss: 5.9619
    Epoch 26/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 35ms/step - loss: 5.8222 - val_loss: 5.5987
    Epoch 27/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 34ms/step - loss: 6.0354 - val_loss: 4.3695
    Epoch 28/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 6.2074 - val_loss: 4.8976
    Epoch 29/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 5.8530 - val_loss: 5.0793
    Epoch 30/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 5.5390 - val_loss: 4.5569
    Epoch 31/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 5.3180 - val_loss: 4.5283
    Epoch 32/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 5.3107 - val_loss: 4.9100
    Epoch 33/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 34ms/step - loss: 5.2554 - val_loss: 5.1411
    Epoch 34/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 33ms/step - loss: 5.2651 - val_loss: 4.6737
    Epoch 35/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 5.2010 - val_loss: 4.2951
    Epoch 36/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 5.1556 - val_loss: 4.4483
    Epoch 37/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.0804 - val_loss: 4.7478
    Epoch 38/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 5.0428 - val_loss: 4.6622
    Epoch 39/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 5.0015 - val_loss: 4.2873
    Epoch 40/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.9445 - val_loss: 4.1144
    Epoch 41/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.8936 - val_loss: 4.2068
    Epoch 42/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 38ms/step - loss: 4.7999 - val_loss: 4.3696
    Epoch 43/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.7322 - val_loss: 3.8969
    Epoch 44/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 4.7025 - val_loss: 3.3501
    Epoch 45/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.6270 - val_loss: 3.5655
    Epoch 46/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.5269 - val_loss: 3.9433
    Epoch 47/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.4715 - val_loss: 3.6484
    Epoch 48/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.4339 - val_loss: 3.2978
    Epoch 49/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 4.4108 - val_loss: 3.4302
    Epoch 50/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 4.3239 - val_loss: 3.5431
    Epoch 51/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 4.2851 - val_loss: 3.3127
    Epoch 52/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 4.2515 - val_loss: 3.2490
    Epoch 53/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 4.1829 - val_loss: 3.3441
    Epoch 54/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 4.1374 - val_loss: 3.3451
    Epoch 55/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 4.0868 - val_loss: 3.2107
    Epoch 56/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 4.0250 - val_loss: 3.1366
    Epoch 57/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 4.0029 - val_loss: 3.0640
    Epoch 58/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 3.9455 - val_loss: 2.9411
    Epoch 59/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 3.9110 - val_loss: 2.9355
    Epoch 60/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 3.8314 - val_loss: 2.9251
    Validation Loss for Interval 13:
    [2608.04443359375, 1924.6578369140625, 1363.2723388671875, 862.7098999023438, 439.736328125, 144.03506469726562, 23.234451293945312, 61.871368408203125, 136.8895263671875, 139.99990844726562, 83.02254486083984, 29.137502670288086, 8.896228790283203, 13.073526382446289, 21.382755279541016, 22.29289436340332, 16.0302677154541, 8.660019874572754, 5.70107889175415, 7.0250725746154785, 8.836477279663086, 8.66220760345459, 7.513368129730225, 6.458014965057373, 5.961892127990723, 5.598719596862793, 4.3695478439331055, 4.897590160369873, 5.079321384429932, 4.556859970092773, 4.528318881988525, 4.910025119781494, 5.141066074371338, 4.6737213134765625, 4.2950568199157715, 4.4482622146606445, 4.747750759124756, 4.662221431732178, 4.287292957305908, 4.114436626434326, 4.2067551612854, 4.369571208953857, 3.8969461917877197, 3.3501439094543457, 3.5654830932617188, 3.9433271884918213, 3.6484241485595703, 3.2977890968322754, 3.430180549621582, 3.5431067943573, 3.31270432472229, 3.2490427494049072, 3.344120502471924, 3.3450546264648438, 3.2106945514678955, 3.1365859508514404, 3.064049243927002, 2.9410910606384277, 2.9354512691497803, 2.925105571746826]
    ========================================
    Decoded Forecasts for Interval 13 (Forecast Date: 2018-01-01):
    PRCP: [7.906506  7.979729  7.3533607 6.943485 ] (Average: 7.55)
    TAVG: [69.243546 69.58154  69.57555  68.10111 ] (Average: 69.13)
    TMAX: [79.71889 80.05884 79.88965 78.4426 ] (Average: 79.53)
    TMIN: [57.52     57.861317 57.852264 56.354374] (Average: 57.40)
    ========================================
    


```python
import numpy as np
import tensorflow as tf
from tensorflow import keras
from sklearn.model_selection import train_test_split
import pandas as pd

# Assuming you have your 'data' prepared and loaded with the appropriate shape

# Convert 'DATE' column to timestamp format
data['DATE'] = pd.to_datetime(data['DATE'])

# Set random seeds for reproducibility
tf.random.set_seed(42)
np.random.seed(42)

# Specify parameters
history_years = 20 # Number of years for historical data
forecast_year = 1   # Number of years to forecast
num_intervals =  13   # Number of intervals to repeat the process
interval_length = 365  # Length of each interval in days

# Calculate the total length of data
total_years = history_years + forecast_year

# Create an empty list to store forecasting results
forecast_results = []

# Create an empty dictionary to store parameter predictions
parameter_predictions = {
    "PRCP": [],
    "TAVG": [],
    "TMAX": [],
    "TMIN": []
}

# Define the initial start date for the intervals
initial_start_date = pd.Timestamp("1985-01-01")

# Loop over different intervals
for interval in range(num_intervals):
    # Calculate the start and end dates for the historical period
    start_date = initial_start_date + pd.DateOffset(years=interval)
    end_date = start_date + pd.DateOffset(years=history_years)
    
    # Extract data for the current historical interval
    historical_data = data[(data['DATE'] >= start_date) & (data['DATE'] < end_date)]
    
    # Calculate the start and end dates for the forecast period
    forecast_start_date = end_date + pd.DateOffset(years=1)  # Add one year for uniform forecasting
    forecast_end_date = forecast_start_date + pd.DateOffset(years=1)
    
    # Extract data for the current forecast interval
    forecast_data = data[(data['DATE'] >= forecast_start_date) & (data['DATE'] < forecast_end_date)]
    
    # Split historical data into train and test sets
    train_data, test_data = train_test_split(historical_data, test_size=0.2, shuffle=False)
    
    # Create Stacked Denoising Autoencoder
    your_input_shape = historical_data.shape[1] - 1  
    your_output_shape = your_input_shape  # Define your output shape here
    
    denoising_encoder = keras.models.Sequential([
        keras.layers.Flatten(input_shape=[your_input_shape]),
        keras.layers.GaussianNoise(0.2),
        keras.layers.Dense(100, activation="selu"),
        keras.layers.Dense(30, activation="selu")
    ])
    
    denoising_decoder = keras.models.Sequential([
        keras.layers.Dense(100, activation="selu", input_shape=[30]),
        keras.layers.Dense(your_output_shape, activation="linear"),  # Use linear activation for output layer
        keras.layers.Reshape([your_output_shape])
    ])
    
    denoising_ae = keras.models.Sequential([denoising_encoder, denoising_decoder])
    denoising_ae.compile(loss="mean_squared_error", optimizer=keras.optimizers.Adam(learning_rate=0.001))
    
    # Train the autoencoder on train data with validation loss monitoring
    history = denoising_ae.fit(train_data.drop('DATE', axis=1), train_data.drop('DATE', axis=1),
                                epochs=60, validation_data=(test_data.drop('DATE', axis=1), test_data.drop('DATE', axis=1)),
                                verbose=1)  # Set verbose to 1 to see training progress
    
    # Display validation loss for each epoch
    print(f"Validation Loss for Interval {interval + 1}:")
    print(history.history['val_loss'])
    print("=" * 40)

    # Use the trained autoencoder for forecasting
    encoded_forecast = denoising_ae.layers[0](forecast_data.drop('DATE', axis=1).values)  # Access encoder layers
    decoded_forecast = denoising_ae.layers[1](encoded_forecast)  # Access decoder layers
    
    # Store the decoded forecast results for this interval
    forecast_results.append(decoded_forecast)

    # Display parameter predictions for this interval
    print(f"Decoded Forecasts for Interval {interval + 1} (Forecast Date: {forecast_start_date.date()}):")
    for param_idx, param_name in enumerate(["PRCP", "TAVG", "TMAX", "TMIN"]):
        param_prediction = decoded_forecast[:, param_idx]
        parameter_predictions[param_name].extend(param_prediction)
        avg_param_prediction = np.mean(param_prediction)  # Calculate average prediction
        print(f"{param_name}: {param_prediction} (Average: {avg_param_prediction:.2f})")
    print("=" * 40)

    # Move the initial start date for the next interval
    initial_start_date += pd.DateOffset(years=0)
    


    


```

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    Epoch 1/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m5s[0m 112ms/step - loss: 3408.4363 - val_loss: 2775.4082
    Epoch 2/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 2460.1348 - val_loss: 1950.9048
    Epoch 3/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 1682.2141 - val_loss: 1163.7905
    Epoch 4/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 950.2823 - val_loss: 479.6435
    Epoch 5/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 347.8693 - val_loss: 70.5891
    Epoch 6/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 40.3056 - val_loss: 56.5226
    Epoch 7/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 68.4957 - val_loss: 127.8639
    Epoch 8/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 108.9242 - val_loss: 59.0354
    Epoch 9/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 43.3895 - val_loss: 9.8783
    Epoch 10/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 10.1068 - val_loss: 17.6060
    Epoch 11/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 17.3448 - val_loss: 26.5904
    Epoch 12/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 20.4342 - val_loss: 19.3779
    Epoch 13/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 12.4265 - val_loss: 10.9342
    Epoch 14/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 7.3086 - val_loss: 9.5538
    Epoch 15/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 8.1639 - val_loss: 9.6302
    Epoch 16/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 8.1297 - val_loss: 8.6712
    Epoch 17/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 6.7983 - val_loss: 9.0119
    Epoch 18/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.6007 - val_loss: 9.7992
    Epoch 19/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 6.8581 - val_loss: 9.4254
    Epoch 20/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 6.5161 - val_loss: 8.5827
    Epoch 21/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 6.2002 - val_loss: 8.2446
    Epoch 22/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 6.1016 - val_loss: 8.2330
    Epoch 23/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.9617 - val_loss: 8.3432
    Epoch 24/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 5.8486 - val_loss: 8.2704
    Epoch 25/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.7307 - val_loss: 8.0184
    Epoch 26/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.5655 - val_loss: 7.8553
    Epoch 27/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 5.4165 - val_loss: 7.6468
    Epoch 28/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.2583 - val_loss: 7.4980
    Epoch 29/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.1342 - val_loss: 7.5679
    Epoch 30/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.0124 - val_loss: 7.4279
    Epoch 31/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 4.7872 - val_loss: 7.4305
    Epoch 32/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.6899 - val_loss: 6.9940
    Epoch 33/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 4.4747 - val_loss: 6.8211
    Epoch 34/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.3878 - val_loss: 6.8702
    Epoch 35/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 4.2624 - val_loss: 6.6719
    Epoch 36/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.1069 - val_loss: 6.5198
    Epoch 37/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 4.0179 - val_loss: 6.2839
    Epoch 38/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 3.8432 - val_loss: 6.0491
    Epoch 39/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 3.7253 - val_loss: 5.9506
    Epoch 40/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 3.6432 - val_loss: 6.0053
    Epoch 41/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.5639 - val_loss: 5.8945
    Epoch 42/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.4877 - val_loss: 5.7292
    Epoch 43/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 3.3646 - val_loss: 5.6491
    Epoch 44/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.2733 - val_loss: 5.5883
    Epoch 45/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.1973 - val_loss: 5.4759
    Epoch 46/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.0993 - val_loss: 5.3707
    Epoch 47/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 2.9597 - val_loss: 5.2889
    Epoch 48/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 2.8446 - val_loss: 5.2505
    Epoch 49/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 2.7907 - val_loss: 5.2155
    Epoch 50/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2.7216 - val_loss: 5.0046
    Epoch 51/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2.6233 - val_loss: 4.9085
    Epoch 52/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 2.5260 - val_loss: 4.9722
    Epoch 53/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 2.4822 - val_loss: 4.8162
    Epoch 54/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 2.3881 - val_loss: 4.6515
    Epoch 55/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2.3207 - val_loss: 4.5617
    Epoch 56/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 2.2730 - val_loss: 4.4308
    Epoch 57/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 2.1784 - val_loss: 4.3667
    Epoch 58/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2.1240 - val_loss: 4.2322
    Epoch 59/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2.0537 - val_loss: 4.0962
    Epoch 60/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 2.0094 - val_loss: 4.0523
    Validation Loss for Interval 1:
    [2775.408203125, 1950.90478515625, 1163.79052734375, 479.64349365234375, 70.5891342163086, 56.52256393432617, 127.86388397216797, 59.0353889465332, 9.878314018249512, 17.60597038269043, 26.590370178222656, 19.377872467041016, 10.934222221374512, 9.553812026977539, 9.630175590515137, 8.671187400817871, 9.011859893798828, 9.799237251281738, 9.425396919250488, 8.582710266113281, 8.244560241699219, 8.232990264892578, 8.34318733215332, 8.270444869995117, 8.018413543701172, 7.855289459228516, 7.646792888641357, 7.497958660125732, 7.567880630493164, 7.4278974533081055, 7.430545330047607, 6.994009017944336, 6.8211445808410645, 6.870235443115234, 6.671858310699463, 6.519820690155029, 6.283901691436768, 6.049053192138672, 5.950562953948975, 6.005306720733643, 5.894536018371582, 5.729236125946045, 5.64914083480835, 5.588306427001953, 5.4759202003479, 5.370693683624268, 5.288946628570557, 5.250521183013916, 5.2155232429504395, 5.004619598388672, 4.908545970916748, 4.972215175628662, 4.816160202026367, 4.651493549346924, 4.561740875244141, 4.4307684898376465, 4.366687774658203, 4.232176303863525, 4.096181869506836, 4.052318572998047]
    ========================================
    Decoded Forecasts for Interval 1 (Forecast Date: 2006-01-01):
    PRCP: [4.743013  4.7312136 4.176712  4.4773107 4.023946  4.638782  8.1429
     8.113513 ] (Average: 5.38)
    TAVG: [69.03182  69.008385 68.11344  66.977005 66.146706 69.230804 69.5415
     69.66665 ] (Average: 68.46)
    TMAX: [81.71029  81.647026 78.661224 77.91638  75.67346  81.70221  82.49899
     82.55527 ] (Average: 80.30)
    TMIN: [56.719524 56.70659  56.435913 55.332047 54.888435 56.939774 57.024414
     57.157948] (Average: 56.40)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m3s[0m 80ms/step - loss: 3229.4043 - val_loss: 2620.6326
    Epoch 2/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 2319.4675 - val_loss: 1719.8306
    Epoch 3/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 1463.7437 - val_loss: 848.8808
    Epoch 4/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 656.8424 - val_loss: 198.2251
    Epoch 5/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 130.3547 - val_loss: 29.7108
    Epoch 6/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 56.6848 - val_loss: 138.4945
    Epoch 7/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 9ms/step - loss: 128.5218 - val_loss: 90.8150
    Epoch 8/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 63.5284 - val_loss: 27.0345
    Epoch 9/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 16.6388 - val_loss: 21.2148
    Epoch 10/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 18.1023 - val_loss: 23.0079
    Epoch 11/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 20.8568 - val_loss: 15.9622
    Epoch 12/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 14.5627 - val_loss: 8.7106
    Epoch 13/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 7.9508 - val_loss: 9.2140
    Epoch 14/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 7.1960 - val_loss: 11.4837
    Epoch 15/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 7.6088 - val_loss: 9.4525
    Epoch 16/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 6.0714 - val_loss: 7.4423
    Epoch 17/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 5.6594 - val_loss: 7.3631
    Epoch 18/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.0799 - val_loss: 7.4620
    Epoch 19/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 5.8320 - val_loss: 7.5084
    Epoch 20/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 5.4369 - val_loss: 7.5513
    Epoch 21/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 5.2907 - val_loss: 7.2439
    Epoch 22/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 5.2037 - val_loss: 6.8089
    Epoch 23/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 9ms/step - loss: 5.0901 - val_loss: 6.8661
    Epoch 24/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 9ms/step - loss: 5.0848 - val_loss: 6.8283
    Epoch 25/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 4.9358 - val_loss: 6.5530
    Epoch 26/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 4.8119 - val_loss: 6.4223
    Epoch 27/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 4.6960 - val_loss: 6.3232
    Epoch 28/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 4.6298 - val_loss: 6.2226
    Epoch 29/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 4.5693 - val_loss: 6.1740
    Epoch 30/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 4.4772 - val_loss: 5.9773
    Epoch 31/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 4.3897 - val_loss: 5.8807
    Epoch 32/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.2895 - val_loss: 5.7552
    Epoch 33/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 4.2219 - val_loss: 5.5869
    Epoch 34/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 4.1127 - val_loss: 5.6150
    Epoch 35/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 4.0164 - val_loss: 5.4715
    Epoch 36/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.9170 - val_loss: 5.3851
    Epoch 37/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 3.8464 - val_loss: 5.2205
    Epoch 38/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 3.7447 - val_loss: 4.9588
    Epoch 39/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.6390 - val_loss: 5.0980
    Epoch 40/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 3.5682 - val_loss: 4.7879
    Epoch 41/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 3.4264 - val_loss: 4.6798
    Epoch 42/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 3.3428 - val_loss: 4.6932
    Epoch 43/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.2595 - val_loss: 4.5471
    Epoch 44/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 3.1945 - val_loss: 4.5036
    Epoch 45/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.1289 - val_loss: 4.4048
    Epoch 46/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.0778 - val_loss: 4.3844
    Epoch 47/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 3.0148 - val_loss: 4.3580
    Epoch 48/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 2.9830 - val_loss: 4.2917
    Epoch 49/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 2.9283 - val_loss: 4.2583
    Epoch 50/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2.8770 - val_loss: 4.1814
    Epoch 51/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 2.8156 - val_loss: 4.1391
    Epoch 52/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 2.7679 - val_loss: 4.1257
    Epoch 53/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 2.7497 - val_loss: 4.0457
    Epoch 54/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 2.6855 - val_loss: 4.0196
    Epoch 55/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2.6324 - val_loss: 3.9492
    Epoch 56/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 2.5897 - val_loss: 3.9056
    Epoch 57/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2.5328 - val_loss: 3.8668
    Epoch 58/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 2.4774 - val_loss: 3.7798
    Epoch 59/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 2.4045 - val_loss: 3.7609
    Epoch 60/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 2.3517 - val_loss: 3.6793
    Validation Loss for Interval 2:
    [2620.632568359375, 1719.83056640625, 848.8807983398438, 198.2250518798828, 29.710752487182617, 138.49453735351562, 90.81499481201172, 27.03453254699707, 21.214794158935547, 23.007915496826172, 15.96218490600586, 8.7106351852417, 9.213991165161133, 11.48371410369873, 9.452493667602539, 7.4423136711120605, 7.363080024719238, 7.461982727050781, 7.508426189422607, 7.5512895584106445, 7.243853569030762, 6.808940887451172, 6.866086483001709, 6.828296661376953, 6.553000450134277, 6.422292709350586, 6.323156356811523, 6.2226152420043945, 6.1739702224731445, 5.9772868156433105, 5.880664348602295, 5.755189418792725, 5.586881637573242, 5.614951133728027, 5.471470832824707, 5.385112285614014, 5.2204718589782715, 4.958780288696289, 5.09800910949707, 4.787883758544922, 4.679814338684082, 4.6931538581848145, 4.547055244445801, 4.503568172454834, 4.404750823974609, 4.384411811828613, 4.358015060424805, 4.291744232177734, 4.2583441734313965, 4.18142032623291, 4.139127731323242, 4.12568998336792, 4.045652866363525, 4.019606590270996, 3.9491875171661377, 3.9055566787719727, 3.866848945617676, 3.779831647872925, 3.7608845233917236, 3.679253578186035]
    ========================================
    Decoded Forecasts for Interval 2 (Forecast Date: 2007-01-01):
    PRCP: [9.781558 9.678138 9.52683  9.216508] (Average: 9.55)
    TAVG: [69.4513   69.167656 68.738815 68.96529 ] (Average: 69.08)
    TMAX: [77.72328 77.61266 77.44902 78.10997] (Average: 77.72)
    TMIN: [56.614838 56.489624 56.29876  56.73589 ] (Average: 56.53)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m3s[0m 93ms/step - loss: 3789.9946 - val_loss: 3113.6606
    Epoch 2/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 2764.6465 - val_loss: 2255.6597
    Epoch 3/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 1962.0618 - val_loss: 1544.3560
    Epoch 4/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 1303.3883 - val_loss: 908.7161
    Epoch 5/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 710.9485 - val_loss: 350.8539
    Epoch 6/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 235.5115 - val_loss: 38.5743
    Epoch 7/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 26.7309 - val_loss: 37.9012
    Epoch 8/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 68.1471 - val_loss: 88.0447
    Epoch 9/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 90.6891 - val_loss: 45.7398
    Epoch 10/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 36.7714 - val_loss: 18.3241
    Epoch 11/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 11.6604 - val_loss: 24.4746
    Epoch 12/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 17.3066 - val_loss: 26.0452
    Epoch 13/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 18.9089 - val_loss: 16.0727
    Epoch 14/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 12.7307 - val_loss: 8.4509
    Epoch 15/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 8.9729 - val_loss: 8.6124
    Epoch 16/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 9.7147 - val_loss: 10.1120
    Epoch 17/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 9.8739 - val_loss: 9.7303
    Epoch 18/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 8.7445 - val_loss: 9.5976
    Epoch 19/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 8.4715 - val_loss: 9.9658
    Epoch 20/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 8.6443 - val_loss: 9.8748
    Epoch 21/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 8.4809 - val_loss: 9.4697
    Epoch 22/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 8.2837 - val_loss: 9.0671
    Epoch 23/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 8.2606 - val_loss: 8.8745
    Epoch 24/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 8.2305 - val_loss: 8.8405
    Epoch 25/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 8.1632 - val_loss: 9.1379
    Epoch 26/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 8.1258 - val_loss: 9.2374
    Epoch 27/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 8.0523 - val_loss: 9.2033
    Epoch 28/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 8.0037 - val_loss: 9.0440
    Epoch 29/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 7.9373 - val_loss: 8.8700
    Epoch 30/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 7.8466 - val_loss: 8.7361
    Epoch 31/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 7.6971 - val_loss: 8.4889
    Epoch 32/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 7.5767 - val_loss: 8.5136
    Epoch 33/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 7.4870 - val_loss: 8.4980
    Epoch 34/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 7.4272 - val_loss: 8.2469
    Epoch 35/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 7.3507 - val_loss: 8.0900
    Epoch 36/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 7.3048 - val_loss: 8.0949
    Epoch 37/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 7.2436 - val_loss: 8.0389
    Epoch 38/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 7.1553 - val_loss: 7.9424
    Epoch 39/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 7.1134 - val_loss: 7.8633
    Epoch 40/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 7.0356 - val_loss: 7.7779
    Epoch 41/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 6.9534 - val_loss: 7.7289
    Epoch 42/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.8775 - val_loss: 7.6303
    Epoch 43/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.8078 - val_loss: 7.5177
    Epoch 44/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.7194 - val_loss: 7.4198
    Epoch 45/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 6.6288 - val_loss: 7.2760
    Epoch 46/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 6.5404 - val_loss: 7.1231
    Epoch 47/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.4809 - val_loss: 7.0838
    Epoch 48/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 6.4003 - val_loss: 7.0262
    Epoch 49/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 6.3183 - val_loss: 6.9027
    Epoch 50/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 6.2348 - val_loss: 6.7855
    Epoch 51/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 6.1653 - val_loss: 6.7124
    Epoch 52/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.0614 - val_loss: 6.5654
    Epoch 53/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 6.0069 - val_loss: 6.4734
    Epoch 54/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.9123 - val_loss: 6.3603
    Epoch 55/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.8102 - val_loss: 6.2702
    Epoch 56/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 5.7146 - val_loss: 6.1523
    Epoch 57/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 5.6402 - val_loss: 5.9929
    Epoch 58/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.5229 - val_loss: 5.8806
    Epoch 59/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.3582 - val_loss: 5.3617
    Epoch 60/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 5.1977 - val_loss: 5.5353
    Validation Loss for Interval 3:
    [3113.66064453125, 2255.65966796875, 1544.35595703125, 908.716064453125, 350.8538818359375, 38.57425308227539, 37.90120315551758, 88.04473876953125, 45.73975372314453, 18.324092864990234, 24.47458267211914, 26.045198440551758, 16.072736740112305, 8.450887680053711, 8.6123628616333, 10.11198616027832, 9.730301856994629, 9.597597122192383, 9.96580982208252, 9.874813079833984, 9.469749450683594, 9.06710433959961, 8.874467849731445, 8.8405179977417, 9.13791561126709, 9.23742389678955, 9.20328140258789, 9.043980598449707, 8.86995792388916, 8.736069679260254, 8.488916397094727, 8.513574600219727, 8.497997283935547, 8.246854782104492, 8.089977264404297, 8.094938278198242, 8.03892993927002, 7.942377090454102, 7.863340377807617, 7.777860164642334, 7.728899002075195, 7.630324363708496, 7.517728328704834, 7.419761657714844, 7.276031494140625, 7.123124122619629, 7.083780765533447, 7.026176929473877, 6.902749061584473, 6.785454750061035, 6.712398052215576, 6.565411567687988, 6.473398685455322, 6.360259056091309, 6.270243167877197, 6.1522955894470215, 5.992918968200684, 5.880566596984863, 5.3617167472839355, 5.535301208496094]
    ========================================
    Decoded Forecasts for Interval 3 (Forecast Date: 2008-01-01):
    PRCP: [5.51608   5.103101  5.1480265] (Average: 5.26)
    TAVG: [68.17693  68.662285 68.6108  ] (Average: 68.48)
    TMAX: [79.22488 79.94354 79.86653] (Average: 79.68)
    TMIN: [56.280346 56.7028   56.657207] (Average: 56.55)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m2s[0m 66ms/step - loss: 3074.8411 - val_loss: 2731.3298
    Epoch 2/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 2475.5940 - val_loss: 2149.3401
    Epoch 3/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 1901.1765 - val_loss: 1466.6843
    Epoch 4/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 1247.5542 - val_loss: 738.8501
    Epoch 5/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 576.3511 - val_loss: 166.5655
    Epoch 6/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 103.8634 - val_loss: 20.5784
    Epoch 7/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 7ms/step - loss: 41.2404 - val_loss: 149.8322
    Epoch 8/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 134.4881 - val_loss: 91.9571
    Epoch 9/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 64.3192 - val_loss: 11.9699
    Epoch 10/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 10.1085 - val_loss: 17.2411
    Epoch 11/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 20.7951 - val_loss: 26.5898
    Epoch 12/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 24.6116 - val_loss: 15.8380
    Epoch 13/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 12.6511 - val_loss: 9.3920
    Epoch 14/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 7.6297 - val_loss: 11.9174
    Epoch 15/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 9.9745 - val_loss: 10.7294
    Epoch 16/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 9.1225 - val_loss: 7.6506
    Epoch 17/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 7.2568 - val_loss: 7.6074
    Epoch 18/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 7.3829 - val_loss: 8.0403
    Epoch 19/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 7.3182 - val_loss: 7.8168
    Epoch 20/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 6.9099 - val_loss: 7.8713
    Epoch 21/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 9ms/step - loss: 6.8123 - val_loss: 7.8512
    Epoch 22/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 6.7926 - val_loss: 7.4626
    Epoch 23/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 6.6330 - val_loss: 7.2152
    Epoch 24/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 6.4964 - val_loss: 7.1417
    Epoch 25/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 6.3943 - val_loss: 7.1009
    Epoch 26/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 6.2538 - val_loss: 7.0081
    Epoch 27/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 6.1777 - val_loss: 6.8066
    Epoch 28/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 6.0659 - val_loss: 6.7676
    Epoch 29/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 6.0127 - val_loss: 6.7203
    Epoch 30/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 5.9156 - val_loss: 6.6131
    Epoch 31/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 5.8215 - val_loss: 6.5384
    Epoch 32/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 5.7312 - val_loss: 6.4743
    Epoch 33/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 5.6685 - val_loss: 6.3432
    Epoch 34/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 5.6149 - val_loss: 6.2344
    Epoch 35/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 5.4981 - val_loss: 6.1572
    Epoch 36/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 5.3820 - val_loss: 6.0434
    Epoch 37/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 5.3292 - val_loss: 6.0116
    Epoch 38/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.1949 - val_loss: 5.8356
    Epoch 39/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.0921 - val_loss: 5.6527
    Epoch 40/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.0003 - val_loss: 5.5684
    Epoch 41/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.9183 - val_loss: 5.3570
    Epoch 42/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 4.8269 - val_loss: 5.2624
    Epoch 43/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 4.7520 - val_loss: 5.1888
    Epoch 44/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 4.6799 - val_loss: 5.0302
    Epoch 45/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 4.5447 - val_loss: 5.0836
    Epoch 46/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 4.5160 - val_loss: 4.9066
    Epoch 47/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 4.3999 - val_loss: 4.8200
    Epoch 48/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 4.3272 - val_loss: 4.7947
    Epoch 49/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 4.2396 - val_loss: 4.6606
    Epoch 50/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 4.1701 - val_loss: 4.5901
    Epoch 51/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 4.0778 - val_loss: 4.4924
    Epoch 52/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 7ms/step - loss: 3.9894 - val_loss: 4.4447
    Epoch 53/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.9078 - val_loss: 4.3824
    Epoch 54/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 3.8612 - val_loss: 4.2275
    Epoch 55/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 3.7718 - val_loss: 4.2501
    Epoch 56/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.6903 - val_loss: 4.0929
    Epoch 57/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.6382 - val_loss: 4.0660
    Epoch 58/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 3.5901 - val_loss: 3.9645
    Epoch 59/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.4934 - val_loss: 3.8817
    Epoch 60/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.4364 - val_loss: 3.8108
    Validation Loss for Interval 4:
    [2731.329833984375, 2149.340087890625, 1466.684326171875, 738.85009765625, 166.5654754638672, 20.578441619873047, 149.8321533203125, 91.95707702636719, 11.969940185546875, 17.241107940673828, 26.589765548706055, 15.838016510009766, 9.392048835754395, 11.917366027832031, 10.729351043701172, 7.650595188140869, 7.607440948486328, 8.040290832519531, 7.816843509674072, 7.8713297843933105, 7.851200580596924, 7.4625701904296875, 7.215244293212891, 7.141700744628906, 7.100890159606934, 7.008099555969238, 6.8066020011901855, 6.767612934112549, 6.720321178436279, 6.613063812255859, 6.538401126861572, 6.474302291870117, 6.343240737915039, 6.2343597412109375, 6.157169818878174, 6.043425559997559, 6.011632442474365, 5.835604190826416, 5.6526947021484375, 5.568357944488525, 5.356974124908447, 5.262397289276123, 5.188816547393799, 5.030184268951416, 5.083591938018799, 4.906640529632568, 4.820031642913818, 4.794704914093018, 4.660564422607422, 4.590142250061035, 4.4923505783081055, 4.444731712341309, 4.382423400878906, 4.227475166320801, 4.250082492828369, 4.092904090881348, 4.065999507904053, 3.964498996734619, 3.8817012310028076, 3.8107802867889404]
    ========================================
    Decoded Forecasts for Interval 4 (Forecast Date: 2009-01-01):
    PRCP: [7.379451  7.3789806 6.6748786 7.4525075 7.4361587 7.377285 ] (Average: 7.28)
    TAVG: [70.34238  70.7073   68.8926   66.661644 66.958534 68.01931 ] (Average: 68.60)
    TMAX: [80.48306  80.886826 78.371635 76.00156  76.319046 77.464325] (Average: 78.25)
    TMIN: [57.45823  57.76828  56.452953 54.57599  54.81895  55.67152 ] (Average: 56.12)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m3s[0m 95ms/step - loss: 2778.3191 - val_loss: 2191.3718
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 1899.9034 - val_loss: 1391.1680
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1161.3573 - val_loss: 689.8309
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 536.4439 - val_loss: 190.8513
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 131.8404 - val_loss: 30.1430
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 45.0185 - val_loss: 114.6298
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 117.5258 - val_loss: 128.4914
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 102.2581 - val_loss: 57.9312
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 40.4128 - val_loss: 27.9618
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 23.7206 - val_loss: 31.5815
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 28.9874 - val_loss: 26.5200
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 23.6075 - val_loss: 14.1843
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 13.4906 - val_loss: 10.5320
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 11.0182 - val_loss: 13.3438
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 12.2471 - val_loss: 11.2758
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 9.9253 - val_loss: 7.5228
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 7.4927 - val_loss: 8.1118
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 7.7425 - val_loss: 9.9111
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 8.2423 - val_loss: 9.2148
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 7.5645 - val_loss: 7.2912
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 6.8472 - val_loss: 6.3649
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 6.5976 - val_loss: 6.0781
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.3491 - val_loss: 6.4859
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.1482 - val_loss: 6.9328
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 5.9778 - val_loss: 6.5103
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.7791 - val_loss: 5.7050
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 5.6380 - val_loss: 5.7059
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 5.4182 - val_loss: 5.5520
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 5.2254 - val_loss: 5.2511
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.0934 - val_loss: 5.2719
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 4.9701 - val_loss: 5.0236
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 4.8271 - val_loss: 4.6669
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 4.7065 - val_loss: 4.6332
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 36ms/step - loss: 4.5605 - val_loss: 4.4938
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 4.4349 - val_loss: 4.3138
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 4.3892 - val_loss: 4.2661
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 4.2272 - val_loss: 4.0873
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 4.1320 - val_loss: 3.9536
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 4.0304 - val_loss: 3.9196
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.9496 - val_loss: 3.8178
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 3.8640 - val_loss: 3.7350
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 3.7713 - val_loss: 3.6179
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.6824 - val_loss: 3.4714
    Epoch 44/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 3.5853 - val_loss: 3.3827
    Epoch 45/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 3.5047 - val_loss: 3.3594
    Epoch 46/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 3.4393 - val_loss: 3.3268
    Epoch 47/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 3.3737 - val_loss: 3.2588
    Epoch 48/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 30ms/step - loss: 3.3174 - val_loss: 3.1987
    Epoch 49/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.2503 - val_loss: 3.1444
    Epoch 50/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.2052 - val_loss: 3.1425
    Epoch 51/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 3.1660 - val_loss: 3.1135
    Epoch 52/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.1500 - val_loss: 3.0981
    Epoch 53/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 3.1154 - val_loss: 3.0724
    Epoch 54/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 3.0966 - val_loss: 3.0611
    Epoch 55/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 3.0750 - val_loss: 3.0599
    Epoch 56/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 3.0672 - val_loss: 3.0484
    Epoch 57/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.0277 - val_loss: 3.0349
    Epoch 58/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.0176 - val_loss: 3.0082
    Epoch 59/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 2.9881 - val_loss: 3.0192
    Epoch 60/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 2.9833 - val_loss: 3.0219
    Validation Loss for Interval 5:
    [2191.371826171875, 1391.16796875, 689.8309326171875, 190.85134887695312, 30.142976760864258, 114.62983703613281, 128.49143981933594, 57.93117141723633, 27.961824417114258, 31.581527709960938, 26.52003288269043, 14.184250831604004, 10.531950950622559, 13.343766212463379, 11.275814056396484, 7.522810459136963, 8.111831665039062, 9.911127090454102, 9.21475601196289, 7.291177272796631, 6.364874839782715, 6.078113555908203, 6.485928058624268, 6.932766914367676, 6.510254383087158, 5.704957008361816, 5.705872058868408, 5.551987648010254, 5.251119136810303, 5.271946907043457, 5.0236005783081055, 4.666876792907715, 4.633238315582275, 4.493759632110596, 4.313802242279053, 4.266051292419434, 4.087324142456055, 3.9535951614379883, 3.9196319580078125, 3.8177905082702637, 3.735018014907837, 3.6179471015930176, 3.4714200496673584, 3.3827195167541504, 3.3593990802764893, 3.326819896697998, 3.258801221847534, 3.1987431049346924, 3.144367218017578, 3.1424505710601807, 3.1134657859802246, 3.098060369491577, 3.072359800338745, 3.0610766410827637, 3.059873342514038, 3.048412322998047, 3.034902572631836, 3.0081820487976074, 3.019240379333496, 3.0219223499298096]
    ========================================
    Decoded Forecasts for Interval 5 (Forecast Date: 2010-01-01):
    PRCP: [9.654831 9.51634  9.496985 9.389667] (Average: 9.51)
    TAVG: [66.016655 70.303444 70.1437   69.08699 ] (Average: 68.89)
    TMAX: [75.87509 80.75981 80.58621 79.46372] (Average: 79.17)
    TMIN: [54.332306 57.91392  57.802647 57.092068] (Average: 56.79)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m3s[0m 101ms/step - loss: 3579.1399 - val_loss: 3200.1313
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 2992.4854 - val_loss: 2681.3958
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2498.1067 - val_loss: 2122.2061
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 1961.3188 - val_loss: 1507.7534
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 1365.0667 - val_loss: 873.6516
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 763.1056 - val_loss: 326.8968
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 274.1218 - val_loss: 35.4835
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 42.1569 - val_loss: 48.9754
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 65.5242 - val_loss: 159.1194
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 128.3879 - val_loss: 137.0877
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 84.8496 - val_loss: 55.0276
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 23.9161 - val_loss: 18.2151
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 11.1242 - val_loss: 17.2575
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 21.0021 - val_loss: 16.6165
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 22.9713 - val_loss: 9.1153
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 14.8994 - val_loss: 4.5922
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 7.7107 - val_loss: 8.3868
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.9095 - val_loss: 13.6545
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 8.1238 - val_loss: 13.4614
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 7.2156 - val_loss: 8.3745
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.8553 - val_loss: 6.4020
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 6.0697 - val_loss: 7.3834
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.7504 - val_loss: 8.0318
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.4817 - val_loss: 7.2567
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 5.4691 - val_loss: 6.6422
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.3986 - val_loss: 6.6623
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.1303 - val_loss: 6.4134
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.0241 - val_loss: 5.9000
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.8813 - val_loss: 5.8937
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.8277 - val_loss: 5.8727
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.7227 - val_loss: 5.5903
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.6267 - val_loss: 5.4603
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.5272 - val_loss: 5.3489
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.4395 - val_loss: 5.0957
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.3769 - val_loss: 4.8755
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.3118 - val_loss: 4.7574
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.1964 - val_loss: 4.5871
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.0951 - val_loss: 4.4695
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.0128 - val_loss: 4.2534
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.9181 - val_loss: 4.0320
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.8460 - val_loss: 3.8520
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.7331 - val_loss: 3.6319
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.6200 - val_loss: 3.5106
    Epoch 44/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.5501 - val_loss: 3.2805
    Epoch 45/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 3.4481 - val_loss: 3.0838
    Epoch 46/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.3254 - val_loss: 2.8484
    Epoch 47/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 32ms/step - loss: 3.2442 - val_loss: 2.6220
    Epoch 48/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 3.1692 - val_loss: 2.4943
    Epoch 49/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 3.0530 - val_loss: 2.2859
    Epoch 50/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 2.9885 - val_loss: 2.1889
    Epoch 51/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 2.9083 - val_loss: 1.9849
    Epoch 52/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 2.8667 - val_loss: 1.9614
    Epoch 53/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 2.7876 - val_loss: 1.8053
    Epoch 54/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 2.7190 - val_loss: 1.7424
    Epoch 55/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2.6823 - val_loss: 1.6200
    Epoch 56/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 2.6283 - val_loss: 1.5653
    Epoch 57/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 2.5861 - val_loss: 1.5348
    Epoch 58/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 2.5483 - val_loss: 1.4760
    Epoch 59/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 2.5158 - val_loss: 1.4480
    Epoch 60/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 2.4814 - val_loss: 1.3622
    Validation Loss for Interval 6:
    [3200.13134765625, 2681.395751953125, 2122.2060546875, 1507.75341796875, 873.651611328125, 326.89678955078125, 35.483497619628906, 48.97541427612305, 159.11935424804688, 137.0877227783203, 55.027557373046875, 18.21514129638672, 17.257549285888672, 16.616464614868164, 9.115341186523438, 4.592247486114502, 8.386778831481934, 13.654470443725586, 13.461408615112305, 8.374462127685547, 6.401951789855957, 7.383410453796387, 8.031844139099121, 7.256731033325195, 6.642157554626465, 6.662263870239258, 6.413403511047363, 5.90001106262207, 5.893691062927246, 5.872687816619873, 5.590302467346191, 5.46033239364624, 5.3488616943359375, 5.095653057098389, 4.875514030456543, 4.757352352142334, 4.587079048156738, 4.469508171081543, 4.253352165222168, 4.032022476196289, 3.8520069122314453, 3.631899356842041, 3.5105721950531006, 3.280531644821167, 3.08378529548645, 2.8483502864837646, 2.6220040321350098, 2.4942667484283447, 2.2858986854553223, 2.188864231109619, 1.984868049621582, 1.9614484310150146, 1.8053408861160278, 1.7423542737960815, 1.6200474500656128, 1.5653425455093384, 1.534843921661377, 1.4759521484375, 1.4480035305023193, 1.362187385559082]
    ========================================
    Decoded Forecasts for Interval 6 (Forecast Date: 2011-01-01):
    PRCP: [8.808844 9.279517 9.549716] (Average: 9.21)
    TAVG: [68.89238 69.57277 68.98605] (Average: 69.15)
    TMAX: [79.81265 80.32357 79.20847] (Average: 79.78)
    TMIN: [57.938545 58.770927 58.264557] (Average: 58.32)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m2s[0m 93ms/step - loss: 3101.9104 - val_loss: 2645.2900
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 2364.0686 - val_loss: 1937.0013
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 1705.0442 - val_loss: 1263.9955
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 1069.5682 - val_loss: 629.9454
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 492.9033 - val_loss: 164.2382
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 106.9696 - val_loss: 8.9084
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 24.3884 - val_loss: 110.0244
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 122.4336 - val_loss: 145.5932
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 121.8663 - val_loss: 59.0989
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 40.6245 - val_loss: 9.9218
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 9.8075 - val_loss: 20.1999
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 22.8024 - val_loss: 28.7651
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 26.6223 - val_loss: 19.9766
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 16.4024 - val_loss: 10.7755
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 8.3089 - val_loss: 9.6278
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 7.4470 - val_loss: 11.1370
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 8.2769 - val_loss: 9.2655
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.9664 - val_loss: 6.3157
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.6742 - val_loss: 5.6356
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.8055 - val_loss: 6.2760
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.9802 - val_loss: 6.6424
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.5858 - val_loss: 6.7098
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.2207 - val_loss: 6.6107
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.0724 - val_loss: 6.2345
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 4.9862 - val_loss: 5.7786
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.9206 - val_loss: 5.4958
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.9254 - val_loss: 5.4094
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.8754 - val_loss: 5.4635
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.8029 - val_loss: 5.5606
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.7345 - val_loss: 5.5299
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.6891 - val_loss: 5.3340
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 4.6158 - val_loss: 5.0975
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.5323 - val_loss: 4.9372
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.4723 - val_loss: 4.8005
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.3969 - val_loss: 4.6431
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.2886 - val_loss: 4.4073
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.1962 - val_loss: 4.3025
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.0878 - val_loss: 4.2057
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 4.0255 - val_loss: 3.9877
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 3.9509 - val_loss: 3.7602
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.9081 - val_loss: 3.7533
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.8115 - val_loss: 3.7513
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.7584 - val_loss: 3.5626
    Epoch 44/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 3.6657 - val_loss: 3.3373
    Epoch 45/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 3.6090 - val_loss: 3.1053
    Epoch 46/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 54ms/step - loss: 3.5024 - val_loss: 2.9948
    Epoch 47/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 46ms/step - loss: 3.4337 - val_loss: 2.9837
    Epoch 48/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 3.3356 - val_loss: 2.8422
    Epoch 49/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 31ms/step - loss: 3.3070 - val_loss: 2.5994
    Epoch 50/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 28ms/step - loss: 3.2179 - val_loss: 2.5503
    Epoch 51/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 57ms/step - loss: 3.1488 - val_loss: 2.4587
    Epoch 52/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 47ms/step - loss: 3.0909 - val_loss: 2.3634
    Epoch 53/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 31ms/step - loss: 3.0503 - val_loss: 2.3704
    Epoch 54/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 42ms/step - loss: 2.9928 - val_loss: 2.3087
    Epoch 55/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 47ms/step - loss: 2.9478 - val_loss: 2.1782
    Epoch 56/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 36ms/step - loss: 2.8932 - val_loss: 2.0733
    Epoch 57/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 36ms/step - loss: 2.8291 - val_loss: 1.9503
    Epoch 58/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 31ms/step - loss: 2.7766 - val_loss: 2.0059
    Epoch 59/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 42ms/step - loss: 2.7280 - val_loss: 1.9273
    Epoch 60/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 47ms/step - loss: 2.6691 - val_loss: 1.8529
    Validation Loss for Interval 7:
    [2645.2900390625, 1937.0013427734375, 1263.9954833984375, 629.9454345703125, 164.23822021484375, 8.908361434936523, 110.02437591552734, 145.5931854248047, 59.098915100097656, 9.9217529296875, 20.199861526489258, 28.76505470275879, 19.97663116455078, 10.775468826293945, 9.62784481048584, 11.137003898620605, 9.265519142150879, 6.315706729888916, 5.635564804077148, 6.275992393493652, 6.642410755157471, 6.709820747375488, 6.610653400421143, 6.234513282775879, 5.778641700744629, 5.495799541473389, 5.409430980682373, 5.463513374328613, 5.560592174530029, 5.52988862991333, 5.334009647369385, 5.097460746765137, 4.937237739562988, 4.8004889488220215, 4.643094062805176, 4.407278060913086, 4.302474498748779, 4.205699443817139, 3.9877431392669678, 3.760181427001953, 3.753296375274658, 3.7513222694396973, 3.5625925064086914, 3.3372809886932373, 3.1052582263946533, 2.994795322418213, 2.9836947917938232, 2.8422188758850098, 2.599372386932373, 2.5503427982330322, 2.458691120147705, 2.3634374141693115, 2.370378017425537, 2.3087217807769775, 2.178178310394287, 2.0733065605163574, 1.9503331184387207, 2.005866289138794, 1.927276849746704, 1.8528835773468018]
    ========================================
    Decoded Forecasts for Interval 7 (Forecast Date: 2012-01-01):
    PRCP: [9.7888775 9.966751  9.526731  9.52335  ] (Average: 9.70)
    TAVG: [70.80621  70.44044  71.34887  71.056076] (Average: 70.91)
    TMAX: [78.31787  77.64052  79.33722  79.299545] (Average: 78.65)
    TMIN: [57.029514 56.825466 57.331142 57.077312] (Average: 57.07)
    ========================================
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    Epoch 1/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m4s[0m 142ms/step - loss: 2996.4282 - val_loss: 2513.3074
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 2300.4663 - val_loss: 1824.4513
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 1641.2722 - val_loss: 1157.0713
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 1006.2197 - val_loss: 590.0419
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 483.7799 - val_loss: 218.5384
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 172.7964 - val_loss: 102.4196
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 91.7901 - val_loss: 93.6562
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 79.2029 - val_loss: 60.7498
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 49.0685 - val_loss: 41.7733
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 40.7601 - val_loss: 44.2939
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 40.9967 - val_loss: 32.8744
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 25.1175 - val_loss: 15.0851
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 8.7251 - val_loss: 10.4946
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 7.6591 - val_loss: 12.9607
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 11.6079 - val_loss: 12.0102
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 9.7077 - val_loss: 11.9893
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 7.3708 - val_loss: 10.0250
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 6.3461 - val_loss: 8.1277
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 6.1329 - val_loss: 8.3384
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 5.8308 - val_loss: 9.2227
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 5.7946 - val_loss: 8.6189
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 5.7548 - val_loss: 7.8169
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.6088 - val_loss: 8.1196
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.4935 - val_loss: 8.5209
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 5.5093 - val_loss: 8.1660
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 5.4773 - val_loss: 7.8679
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 5.3870 - val_loss: 8.0189
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 5.3298 - val_loss: 7.9541
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.2929 - val_loss: 7.6720
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 5.2117 - val_loss: 7.6458
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 5.1661 - val_loss: 7.7079
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 5.1371 - val_loss: 7.5759
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 5.0784 - val_loss: 7.4096
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 5.0316 - val_loss: 7.4296
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.0057 - val_loss: 7.4168
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 4.9596 - val_loss: 7.2849
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 4.8998 - val_loss: 7.1616
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 4.8779 - val_loss: 7.1184
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 4.8008 - val_loss: 7.0787
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 4.7532 - val_loss: 6.9252
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 4.6878 - val_loss: 6.5823
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 4.5836 - val_loss: 6.6418
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 4.5238 - val_loss: 6.8158
    Epoch 44/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.4355 - val_loss: 6.5100
    Epoch 45/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 4.3831 - val_loss: 6.2525
    Epoch 46/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 4.3288 - val_loss: 6.2704
    Epoch 47/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 29ms/step - loss: 4.2484 - val_loss: 6.3775
    Epoch 48/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 4.1743 - val_loss: 6.0642
    Epoch 49/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 4.1298 - val_loss: 6.0489
    Epoch 50/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 4.0596 - val_loss: 5.9553
    Epoch 51/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 3.9932 - val_loss: 5.6568
    Epoch 52/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 3.8850 - val_loss: 5.7533
    Epoch 53/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 19ms/step - loss: 3.8213 - val_loss: 5.7877
    Epoch 54/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 3.7706 - val_loss: 5.4861
    Epoch 55/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 3.6748 - val_loss: 5.3540
    Epoch 56/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 3.5518 - val_loss: 5.3956
    Epoch 57/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 3.4642 - val_loss: 5.2370
    Epoch 58/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 3.4201 - val_loss: 5.0202
    Epoch 59/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 3.3551 - val_loss: 5.0468
    Epoch 60/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 3.2921 - val_loss: 4.9292
    Validation Loss for Interval 8:
    [2513.307373046875, 1824.4512939453125, 1157.0712890625, 590.0418701171875, 218.53843688964844, 102.4195785522461, 93.65620422363281, 60.74979782104492, 41.77332305908203, 44.29392623901367, 32.87444305419922, 15.085088729858398, 10.494572639465332, 12.960716247558594, 12.010210037231445, 11.989275932312012, 10.025014877319336, 8.127657890319824, 8.338421821594238, 9.222655296325684, 8.61890983581543, 7.816914081573486, 8.119647979736328, 8.520890235900879, 8.165952682495117, 7.86792516708374, 8.018906593322754, 7.954071521759033, 7.671952247619629, 7.645751476287842, 7.707892417907715, 7.575915813446045, 7.409576416015625, 7.429576396942139, 7.416780948638916, 7.284865379333496, 7.161613941192627, 7.118397235870361, 7.0786638259887695, 6.92521333694458, 6.582276344299316, 6.641758441925049, 6.815772533416748, 6.510019779205322, 6.252547264099121, 6.270362854003906, 6.37750768661499, 6.064202785491943, 6.048934459686279, 5.955310344696045, 5.656836032867432, 5.753344535827637, 5.7876667976379395, 5.486129283905029, 5.353955268859863, 5.3955512046813965, 5.237004280090332, 5.020205974578857, 5.046825408935547, 4.929154396057129]
    ========================================
    Decoded Forecasts for Interval 8 (Forecast Date: 2013-01-01):
    PRCP: [5.4974685] (Average: 5.50)
    TAVG: [69.064316] (Average: 69.06)
    TMAX: [80.04518] (Average: 80.05)
    TMIN: [56.23905] (Average: 56.24)
    ========================================
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    Epoch 1/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m4s[0m 90ms/step - loss: 2796.6814 - val_loss: 2221.6501
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2015.4496 - val_loss: 1522.9548
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1358.6321 - val_loss: 924.1772
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 797.7339 - val_loss: 433.2979
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 356.5525 - val_loss: 144.0002
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 114.9609 - val_loss: 79.8579
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 71.8784 - val_loss: 109.2005
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 86.8249 - val_loss: 86.9645
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 60.9391 - val_loss: 42.1409
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 29.9138 - val_loss: 28.0126
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 24.3211 - val_loss: 28.0856
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 24.7326 - val_loss: 20.9333
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 16.8183 - val_loss: 11.6183
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 8.0606 - val_loss: 10.2519
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 6.3524 - val_loss: 14.4810
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 8.3846 - val_loss: 15.8353
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 8.0815 - val_loss: 13.0152
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 6.0265 - val_loss: 10.4273
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.1780 - val_loss: 9.8708
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.5581 - val_loss: 9.9570
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 5.6811 - val_loss: 9.8244
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.4086 - val_loss: 9.8410
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 5.2163 - val_loss: 10.0825
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.1635 - val_loss: 10.1556
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.0878 - val_loss: 9.9388
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.0101 - val_loss: 9.6638
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.9929 - val_loss: 9.4678
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 4.9625 - val_loss: 9.4044
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 4.9220 - val_loss: 9.4262
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 4.8898 - val_loss: 9.4093
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 4.8846 - val_loss: 9.3281
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 4.8452 - val_loss: 9.2466
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 9ms/step - loss: 4.8232 - val_loss: 9.1523
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.7864 - val_loss: 9.0850
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 4.7215 - val_loss: 9.1128
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 4.6906 - val_loss: 8.0650
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.6038 - val_loss: 8.2073
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 4.5790 - val_loss: 8.7609
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 4.6185 - val_loss: 8.3676
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 4.5703 - val_loss: 8.0475
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 4.5368 - val_loss: 8.3348
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 4.5457 - val_loss: 8.3149
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 13ms/step - loss: 4.5292 - val_loss: 8.0401
    Epoch 44/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.4820 - val_loss: 7.9301
    Epoch 45/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.4358 - val_loss: 7.8936
    Epoch 46/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.4197 - val_loss: 7.7858
    Epoch 47/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 22ms/step - loss: 4.4052 - val_loss: 7.7554
    Epoch 48/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 4.3782 - val_loss: 7.7956
    Epoch 49/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 9ms/step - loss: 4.3603 - val_loss: 7.7107
    Epoch 50/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.3226 - val_loss: 7.4760
    Epoch 51/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.2563 - val_loss: 7.4306
    Epoch 52/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 4.2213 - val_loss: 7.4681
    Epoch 53/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 17ms/step - loss: 4.2044 - val_loss: 7.2504
    Epoch 54/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 4.1577 - val_loss: 6.9902
    Epoch 55/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 4.0931 - val_loss: 6.9309
    Epoch 56/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 26ms/step - loss: 4.0697 - val_loss: 6.8299
    Epoch 57/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 4.0239 - val_loss: 6.8050
    Epoch 58/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.0146 - val_loss: 6.7612
    Epoch 59/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.0136 - val_loss: 6.6123
    Epoch 60/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.9738 - val_loss: 6.4086
    Validation Loss for Interval 9:
    [2221.650146484375, 1522.954833984375, 924.17724609375, 433.2978820800781, 144.000244140625, 79.85789489746094, 109.20050811767578, 86.96451568603516, 42.14086151123047, 28.012622833251953, 28.085609436035156, 20.93332290649414, 11.618318557739258, 10.25191879272461, 14.481043815612793, 15.83530044555664, 13.015213966369629, 10.427277565002441, 9.870768547058105, 9.95700454711914, 9.824371337890625, 9.841017723083496, 10.082539558410645, 10.155620574951172, 9.938814163208008, 9.66384506225586, 9.467835426330566, 9.404375076293945, 9.426192283630371, 9.40926742553711, 9.328124046325684, 9.246623992919922, 9.152313232421875, 9.08501148223877, 9.11284351348877, 8.064986228942871, 8.207277297973633, 8.760893821716309, 8.367594718933105, 8.047527313232422, 8.334798812866211, 8.314852714538574, 8.040141105651855, 7.930083751678467, 7.893613815307617, 7.785791397094727, 7.755356788635254, 7.795565605163574, 7.71073579788208, 7.476003646850586, 7.430573463439941, 7.468075275421143, 7.250368595123291, 6.990218162536621, 6.930886268615723, 6.829870700836182, 6.804956436157227, 6.761196136474609, 6.612253189086914, 6.408556938171387]
    ========================================
    Decoded Forecasts for Interval 9 (Forecast Date: 2014-01-01):
    PRCP: [5.579501  5.4152803 5.195875  5.157032 ] (Average: 5.34)
    TAVG: [70.256615 69.648415 68.82898  68.549614] (Average: 69.32)
    TMAX: [81.20462  80.752045 80.145294 79.75342 ] (Average: 80.46)
    TMIN: [58.59294  58.140152 57.53064  57.352425] (Average: 57.90)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m2s[0m 78ms/step - loss: 2629.8213 - val_loss: 2013.4677
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 1873.0460 - val_loss: 1300.3383
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 1188.9357 - val_loss: 652.7553
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 573.6267 - val_loss: 178.7406
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 141.5203 - val_loss: 13.1788
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 16.7398 - val_loss: 133.8951
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 118.0945 - val_loss: 168.5958
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 120.0073 - val_loss: 69.5605
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 37.4253 - val_loss: 12.2630
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.6269 - val_loss: 15.4452
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 19.1390 - val_loss: 23.8479
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 25.5218 - val_loss: 17.3219
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 16.3272 - val_loss: 10.1220
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 7.0210 - val_loss: 12.8542
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.5123 - val_loss: 18.1406
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 8.8063 - val_loss: 16.8604
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 7.7473 - val_loss: 12.0007
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.6199 - val_loss: 9.5627
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.4440 - val_loss: 9.6862
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.9409 - val_loss: 10.1678
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.7543 - val_loss: 10.4002
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.3725 - val_loss: 10.7055
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.3158 - val_loss: 10.9475
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.3429 - val_loss: 10.8518
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.2943 - val_loss: 10.5021
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.2237 - val_loss: 10.1404
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.2264 - val_loss: 9.9604
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.2347 - val_loss: 10.0189
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.1812 - val_loss: 10.0194
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.0854 - val_loss: 9.8703
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.0254 - val_loss: 9.8052
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.0193 - val_loss: 9.8884
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.9827 - val_loss: 9.8372
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.9464 - val_loss: 9.6613
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.9362 - val_loss: 9.6291
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.9379 - val_loss: 9.6854
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.9254 - val_loss: 9.6722
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.8952 - val_loss: 9.5353
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.8730 - val_loss: 9.4081
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.8582 - val_loss: 9.3993
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 4.8442 - val_loss: 9.4235
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.8145 - val_loss: 9.3433
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.7968 - val_loss: 9.1769
    Epoch 44/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.7686 - val_loss: 9.1625
    Epoch 45/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.7594 - val_loss: 9.2087
    Epoch 46/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 4.7144 - val_loss: 9.0914
    Epoch 47/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.7053 - val_loss: 8.9370
    Epoch 48/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.6705 - val_loss: 8.8368
    Epoch 49/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.6523 - val_loss: 8.8582
    Epoch 50/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.6191 - val_loss: 8.8074
    Epoch 51/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.6008 - val_loss: 8.4554
    Epoch 52/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.5798 - val_loss: 8.4121
    Epoch 53/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.5522 - val_loss: 8.5700
    Epoch 54/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.5281 - val_loss: 8.5313
    Epoch 55/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.5191 - val_loss: 8.3051
    Epoch 56/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.4809 - val_loss: 8.3128
    Epoch 57/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.4590 - val_loss: 8.2315
    Epoch 58/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.4199 - val_loss: 8.1609
    Epoch 59/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.3990 - val_loss: 8.2257
    Epoch 60/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 4.3865 - val_loss: 8.0329
    Validation Loss for Interval 10:
    [2013.4676513671875, 1300.3382568359375, 652.7553100585938, 178.74063110351562, 13.178776741027832, 133.8951416015625, 168.59576416015625, 69.56049346923828, 12.262974739074707, 15.445242881774902, 23.847867965698242, 17.32193946838379, 10.121966361999512, 12.854174613952637, 18.14057731628418, 16.860382080078125, 12.000715255737305, 9.562726020812988, 9.686190605163574, 10.167750358581543, 10.400164604187012, 10.705499649047852, 10.947527885437012, 10.851832389831543, 10.502140045166016, 10.140393257141113, 9.960367202758789, 10.018900871276855, 10.019431114196777, 9.870285987854004, 9.805153846740723, 9.888372421264648, 9.837153434753418, 9.661267280578613, 9.629117965698242, 9.685356140136719, 9.672178268432617, 9.535301208496094, 9.408130645751953, 9.399285316467285, 9.423480987548828, 9.34330940246582, 9.176876068115234, 9.162542343139648, 9.2086763381958, 9.091410636901855, 8.936963081359863, 8.836784362792969, 8.858209609985352, 8.807435035705566, 8.455438613891602, 8.41210651397705, 8.570038795471191, 8.53125286102295, 8.3051176071167, 8.312768936157227, 8.231527328491211, 8.160881042480469, 8.225696563720703, 8.03287410736084]
    ========================================
    Decoded Forecasts for Interval 10 (Forecast Date: 2015-01-01):
    PRCP: [5.2457576 5.2134414 5.23253   5.145986 ] (Average: 5.21)
    TAVG: [72.35888  71.887825 71.33933  69.88296 ] (Average: 71.37)
    TMAX: [84.80664  84.12125  83.290215 81.26681 ] (Average: 83.37)
    TMIN: [60.820557 60.46995  60.148613 59.091084] (Average: 60.13)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m2s[0m 109ms/step - loss: 3978.2122 - val_loss: 3432.5815
    Epoch 2/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3285.3281 - val_loss: 2919.0544
    Epoch 3/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2810.7068 - val_loss: 2539.3577
    Epoch 4/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2439.5127 - val_loss: 2178.0940
    Epoch 5/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 2088.7383 - val_loss: 1827.4353
    Epoch 6/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1740.3643 - val_loss: 1468.9601
    Epoch 7/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1381.2782 - val_loss: 1090.8268
    Epoch 8/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1006.3353 - val_loss: 720.0557
    Epoch 9/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 646.0940 - val_loss: 391.4763
    Epoch 10/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 334.8156 - val_loss: 144.9863
    Epoch 11/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 112.3878 - val_loss: 20.4336
    Epoch 12/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 14.5146 - val_loss: 26.3181
    Epoch 13/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 34.9451 - val_loss: 94.1746
    Epoch 14/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 93.3168 - val_loss: 124.1314
    Epoch 15/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 107.8708 - val_loss: 94.2855
    Epoch 16/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 74.3892 - val_loss: 46.4204
    Epoch 17/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 32.3153 - val_loss: 16.6591
    Epoch 18/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 9.7080 - val_loss: 10.3229
    Epoch 19/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 7.5604 - val_loss: 15.5063
    Epoch 20/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 14.0669 - val_loss: 20.5912
    Epoch 21/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 18.6267 - val_loss: 20.3505
    Epoch 22/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 17.9311 - val_loss: 16.0999
    Epoch 23/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 13.5991 - val_loss: 11.5447
    Epoch 24/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 8.8396 - val_loss: 9.3787
    Epoch 25/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.4523 - val_loss: 9.7518
    Epoch 26/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.4011 - val_loss: 11.0829
    Epoch 27/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 7.2715 - val_loss: 11.7002
    Epoch 28/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 7.5892 - val_loss: 11.3376
    Epoch 29/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 7.1160 - val_loss: 10.5306
    Epoch 30/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.4064 - val_loss: 9.8751
    Epoch 31/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.9999 - val_loss: 9.5479
    Epoch 32/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.9917 - val_loss: 9.3804
    Epoch 33/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.1155 - val_loss: 9.2907
    Epoch 34/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.1698 - val_loss: 9.2135
    Epoch 35/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.1278 - val_loss: 9.1133
    Epoch 36/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.0064 - val_loss: 9.0561
    Epoch 37/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.9321 - val_loss: 9.1359
    Epoch 38/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.9129 - val_loss: 9.2825
    Epoch 39/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.9179 - val_loss: 9.3814
    Epoch 40/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.9189 - val_loss: 9.3855
    Epoch 41/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.8928 - val_loss: 9.2602
    Epoch 42/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.8673 - val_loss: 9.1253
    Epoch 43/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.8419 - val_loss: 9.1214
    Epoch 44/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.8513 - val_loss: 9.1488
    Epoch 45/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.8528 - val_loss: 9.1292
    Epoch 46/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.8463 - val_loss: 9.0401
    Epoch 47/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.8432 - val_loss: 8.9853
    Epoch 48/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.8389 - val_loss: 9.0154
    Epoch 49/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.8219 - val_loss: 9.0642
    Epoch 50/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.8055 - val_loss: 9.0838
    Epoch 51/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.8077 - val_loss: 9.0416
    Epoch 52/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.8078 - val_loss: 8.9643
    Epoch 53/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 5.7843 - val_loss: 8.9398
    Epoch 54/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 5.7763 - val_loss: 8.9717
    Epoch 55/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.7722 - val_loss: 8.9685
    Epoch 56/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 5.7881 - val_loss: 8.8996
    Epoch 57/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 18ms/step - loss: 5.7540 - val_loss: 8.9237
    Epoch 58/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 25ms/step - loss: 5.7565 - val_loss: 8.8888
    Epoch 59/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 24ms/step - loss: 5.7417 - val_loss: 8.8227
    Epoch 60/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.7446 - val_loss: 8.8540
    Validation Loss for Interval 11:
    [3432.58154296875, 2919.054443359375, 2539.357666015625, 2178.093994140625, 1827.435302734375, 1468.9600830078125, 1090.8267822265625, 720.0557250976562, 391.47625732421875, 144.9862823486328, 20.433626174926758, 26.318056106567383, 94.17464447021484, 124.1314468383789, 94.28551483154297, 46.420352935791016, 16.65912628173828, 10.32292366027832, 15.506285667419434, 20.5911865234375, 20.35049819946289, 16.099939346313477, 11.544720649719238, 9.378737449645996, 9.75184154510498, 11.082932472229004, 11.70024299621582, 11.337625503540039, 10.530632019042969, 9.875103950500488, 9.547928810119629, 9.380402565002441, 9.290689468383789, 9.213521957397461, 9.113312721252441, 9.05606460571289, 9.135921478271484, 9.282517433166504, 9.381426811218262, 9.385539054870605, 9.260237693786621, 9.125311851501465, 9.121383666992188, 9.148797988891602, 9.12923812866211, 9.040107727050781, 8.985306739807129, 9.015393257141113, 9.064248085021973, 9.083819389343262, 9.041603088378906, 8.964276313781738, 8.939789772033691, 8.97174072265625, 8.968472480773926, 8.899577140808105, 8.923685073852539, 8.888771057128906, 8.822693824768066, 8.853972434997559]
    ========================================
    Decoded Forecasts for Interval 11 (Forecast Date: 2016-01-01):
    PRCP: [4.8778944] (Average: 4.88)
    TAVG: [68.94822] (Average: 68.95)
    TMAX: [79.50026] (Average: 79.50)
    TMIN: [57.18229] (Average: 57.18)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m2s[0m 117ms/step - loss: 3372.7061 - val_loss: 2980.6250
    Epoch 2/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2797.5706 - val_loss: 2409.6814
    Epoch 3/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2243.5195 - val_loss: 1889.8735
    Epoch 4/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1744.0858 - val_loss: 1389.9216
    Epoch 5/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1266.4629 - val_loss: 921.7891
    Epoch 6/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 830.6598 - val_loss: 537.3656
    Epoch 7/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 484.3377 - val_loss: 272.6140
    Epoch 8/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 252.0719 - val_loss: 136.3581
    Epoch 9/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 133.9505 - val_loss: 92.2939
    Epoch 10/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 90.9249 - val_loss: 75.2033
    Epoch 11/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 66.9601 - val_loss: 53.0264
    Epoch 12/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 43.8676 - val_loss: 35.3165
    Epoch 13/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 29.6800 - val_loss: 27.4552
    Epoch 14/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 26.3035 - val_loss: 29.3710
    Epoch 15/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 29.2550 - val_loss: 30.5965
    Epoch 16/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 28.3688 - val_loss: 25.1865
    Epoch 17/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 20.9171 - val_loss: 16.0350
    Epoch 18/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 11.5883 - val_loss: 9.0431
    Epoch 19/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.3386 - val_loss: 7.0418
    Epoch 20/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.5059 - val_loss: 8.0030
    Epoch 21/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 8.7322 - val_loss: 8.5306
    Epoch 22/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 9.3362 - val_loss: 7.9655
    Epoch 23/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 8.0438 - val_loss: 7.5231
    Epoch 24/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.7266 - val_loss: 7.5098
    Epoch 25/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.1260 - val_loss: 7.2453
    Epoch 26/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.9049 - val_loss: 6.5146
    Epoch 27/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.6988 - val_loss: 5.8227
    Epoch 28/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.6012 - val_loss: 5.6272
    Epoch 29/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.6264 - val_loss: 5.7807
    Epoch 30/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.6553 - val_loss: 5.8038
    Epoch 31/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.5468 - val_loss: 5.6209
    Epoch 32/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.3601 - val_loss: 5.4393
    Epoch 33/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.2752 - val_loss: 5.3862
    Epoch 34/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.2438 - val_loss: 5.3978
    Epoch 35/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.2564 - val_loss: 5.3402
    Epoch 36/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.1770 - val_loss: 5.2048
    Epoch 37/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.1610 - val_loss: 5.0873
    Epoch 38/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.1068 - val_loss: 5.0472
    Epoch 39/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.0797 - val_loss: 5.0206
    Epoch 40/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.0342 - val_loss: 4.9452
    Epoch 41/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.0113 - val_loss: 4.9053
    Epoch 42/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.9750 - val_loss: 4.8612
    Epoch 43/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.9568 - val_loss: 4.8237
    Epoch 44/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 4.9111 - val_loss: 4.7900
    Epoch 45/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 4.8834 - val_loss: 4.7410
    Epoch 46/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 4.8515 - val_loss: 4.6681
    Epoch 47/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.8181 - val_loss: 4.5912
    Epoch 48/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.7951 - val_loss: 4.5294
    Epoch 49/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.8040 - val_loss: 4.4947
    Epoch 50/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 4.7381 - val_loss: 4.4591
    Epoch 51/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 4.7079 - val_loss: 4.4093
    Epoch 52/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.6821 - val_loss: 4.3722
    Epoch 53/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 4.6559 - val_loss: 4.2972
    Epoch 54/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 4.6311 - val_loss: 4.2199
    Epoch 55/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 4.5797 - val_loss: 4.1713
    Epoch 56/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.5865 - val_loss: 4.1485
    Epoch 57/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.5259 - val_loss: 4.0587
    Epoch 58/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.5080 - val_loss: 3.9731
    Epoch 59/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 4.4672 - val_loss: 3.9528
    Epoch 60/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 4.4452 - val_loss: 3.9179
    Validation Loss for Interval 12:
    [2980.625, 2409.681396484375, 1889.87353515625, 1389.921630859375, 921.7891235351562, 537.3656005859375, 272.6139831542969, 136.35813903808594, 92.2939224243164, 75.20332336425781, 53.026363372802734, 35.31648254394531, 27.455244064331055, 29.370960235595703, 30.596473693847656, 25.1865234375, 16.03502082824707, 9.043096542358398, 7.041831970214844, 8.002968788146973, 8.530588150024414, 7.965497970581055, 7.52310037612915, 7.509796142578125, 7.245288372039795, 6.514606952667236, 5.822687149047852, 5.627212047576904, 5.780696392059326, 5.803756237030029, 5.620880603790283, 5.439282417297363, 5.3862199783325195, 5.39777946472168, 5.340227127075195, 5.204811096191406, 5.0873003005981445, 5.047163486480713, 5.020617485046387, 4.945215225219727, 4.905283451080322, 4.861184120178223, 4.823723316192627, 4.790009021759033, 4.740991115570068, 4.668090343475342, 4.591236591339111, 4.529412269592285, 4.494665145874023, 4.45912504196167, 4.409329414367676, 4.372190475463867, 4.297205924987793, 4.219920635223389, 4.171309947967529, 4.1485490798950195, 4.0587334632873535, 3.973107099533081, 3.9527647495269775, 3.917919158935547]
    ========================================
    Decoded Forecasts for Interval 12 (Forecast Date: 2017-01-01):
    PRCP: [7.4969115 7.7053847 7.400827 ] (Average: 7.53)
    TAVG: [69.04476 70.15322 68.66847] (Average: 69.29)
    TMAX: [79.41776  80.73807  78.971466] (Average: 79.71)
    TMIN: [57.050102 58.125042 56.68807 ] (Average: 57.29)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m3s[0m 117ms/step - loss: 3765.5337 - val_loss: 3101.4771
    Epoch 2/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2808.8367 - val_loss: 2225.1069
    Epoch 3/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2005.5814 - val_loss: 1525.0925
    Epoch 4/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1370.7917 - val_loss: 935.2022
    Epoch 5/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 835.6638 - val_loss: 475.1958
    Epoch 6/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 421.4961 - val_loss: 160.8048
    Epoch 7/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 143.4192 - val_loss: 11.2208
    Epoch 8/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 19.7286 - val_loss: 36.0414
    Epoch 9/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 47.5014 - val_loss: 131.2658
    Epoch 10/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 119.6450 - val_loss: 153.5106
    Epoch 11/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 123.9544 - val_loss: 94.8309
    Epoch 12/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 69.1933 - val_loss: 32.8286
    Epoch 13/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 22.3891 - val_loss: 5.2339
    Epoch 14/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 7.6750 - val_loss: 6.2308
    Epoch 15/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 13.6375 - val_loss: 15.2741
    Epoch 16/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 21.9970 - val_loss: 19.6498
    Epoch 17/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 23.5840 - val_loss: 17.3933
    Epoch 18/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 18.2843 - val_loss: 12.3663
    Epoch 19/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 11.4528 - val_loss: 8.7817
    Epoch 20/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 7.2850 - val_loss: 8.0775
    Epoch 21/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.7936 - val_loss: 8.8467
    Epoch 22/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 8.0775 - val_loss: 8.9708
    Epoch 23/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 8.7274 - val_loss: 7.7864
    Epoch 24/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 8.0531 - val_loss: 6.2883
    Epoch 25/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.9419 - val_loss: 5.6283
    Epoch 26/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.3016 - val_loss: 5.9225
    Epoch 27/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.4061 - val_loss: 6.4256
    Epoch 28/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.7605 - val_loss: 6.4844
    Epoch 29/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.7584 - val_loss: 6.1001
    Epoch 30/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.4939 - val_loss: 5.6812
    Epoch 31/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.2859 - val_loss: 5.5220
    Epoch 32/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.1705 - val_loss: 5.6174
    Epoch 33/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.2087 - val_loss: 5.7865
    Epoch 34/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.1887 - val_loss: 5.8862
    Epoch 35/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.1423 - val_loss: 5.8658
    Epoch 36/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.1177 - val_loss: 5.7294
    Epoch 37/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.0649 - val_loss: 5.4953
    Epoch 38/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.0402 - val_loss: 5.2489
    Epoch 39/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.9774 - val_loss: 5.1466
    Epoch 40/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.9452 - val_loss: 5.1580
    Epoch 41/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.8129 - val_loss: 5.3091
    Epoch 42/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.7458 - val_loss: 5.4903
    Epoch 43/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.6857 - val_loss: 5.5722
    Epoch 44/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.6624 - val_loss: 5.5013
    Epoch 45/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.6412 - val_loss: 5.3604
    Epoch 46/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.6062 - val_loss: 5.2906
    Epoch 47/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.5544 - val_loss: 5.3409
    Epoch 48/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.5307 - val_loss: 5.2377
    Epoch 49/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.5043 - val_loss: 4.9808
    Epoch 50/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.4538 - val_loss: 4.6714
    Epoch 51/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.3823 - val_loss: 4.7559
    Epoch 52/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.3505 - val_loss: 4.9262
    Epoch 53/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.3540 - val_loss: 4.7141
    Epoch 54/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.3106 - val_loss: 4.6916
    Epoch 55/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.2661 - val_loss: 4.8578
    Epoch 56/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.2583 - val_loss: 4.6705
    Epoch 57/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.1929 - val_loss: 4.5754
    Epoch 58/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.1803 - val_loss: 4.5790
    Epoch 59/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.1733 - val_loss: 4.4401
    Epoch 60/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.0978 - val_loss: 4.4076
    Validation Loss for Interval 13:
    [3101.47705078125, 2225.10693359375, 1525.092529296875, 935.2022094726562, 475.1957702636719, 160.8047637939453, 11.220794677734375, 36.04142761230469, 131.26583862304688, 153.51060485839844, 94.8309097290039, 32.82861328125, 5.233923435211182, 6.230759620666504, 15.274104118347168, 19.649845123291016, 17.393346786499023, 12.366318702697754, 8.781684875488281, 8.077469825744629, 8.846673965454102, 8.97081470489502, 7.786396026611328, 6.2882609367370605, 5.628317832946777, 5.922541618347168, 6.425550937652588, 6.484350204467773, 6.100124359130859, 5.681161403656006, 5.522037982940674, 5.617362976074219, 5.786458492279053, 5.886180877685547, 5.865769386291504, 5.7294416427612305, 5.495270729064941, 5.248922824859619, 5.146569728851318, 5.157968521118164, 5.309055328369141, 5.490272045135498, 5.572182655334473, 5.501282215118408, 5.36044454574585, 5.290626049041748, 5.340859889984131, 5.237707614898682, 4.980799674987793, 4.671399116516113, 4.755918025970459, 4.926168441772461, 4.714055061340332, 4.6916093826293945, 4.857842922210693, 4.6704583168029785, 4.575375556945801, 4.579010963439941, 4.440091133117676, 4.40762186050415]
    ========================================
    Decoded Forecasts for Interval 13 (Forecast Date: 2018-01-01):
    PRCP: [7.023422  7.0785427 6.814232  6.599268 ] (Average: 6.88)
    TAVG: [69.86263  70.18493  69.973305 68.54316 ] (Average: 69.64)
    TMAX: [80.18172  80.58917  80.26243  78.529305] (Average: 79.89)
    TMIN: [58.007236 58.429317 58.207767 56.4123  ] (Average: 57.76)
    ========================================
    5/5 [==============================] - 0s 22ms/step - loss: 10.2063 - val_loss: 11.5649
    Epoch 16/60
    5/5 [==============================] - 0s 14ms/step - loss: 9.0139 - val_loss: 9.5230
    Epoch 17/60
    5/5 [==============================] - 0s 13ms/step - loss: 7.8249 - val_loss: 8.8681
    Epoch 18/60
    5/5 [==============================] - 0s 16ms/step - loss: 8.0201 - val_loss: 8.2259
    Epoch 19/60
    5/5 [==============================] - 0s 16ms/step - loss: 8.0445 - val_loss: 7.4549
    Epoch 20/60
    5/5 [==============================] - 0s 14ms/step - loss: 7.6265 - val_loss: 8.6187
    Epoch 21/60
    5/5 [==============================] - 0s 16ms/step - loss: 7.5113 - val_loss: 8.7375
    Epoch 22/60
    5/5 [==============================] - 0s 17ms/step - loss: 7.4449 - val_loss: 8.6396
    Epoch 23/60
    5/5 [==============================] - 0s 14ms/step - loss: 7.3355 - val_loss: 8.5817
    Epoch 24/60
    5/5 [==============================] - 0s 13ms/step - loss: 7.1597 - val_loss: 7.7340
    Epoch 25/60
    5/5 [==============================] - 0s 16ms/step - loss: 6.9709 - val_loss: 7.6337
    Epoch 26/60
    5/5 [==============================] - 0s 13ms/step - loss: 6.8033 - val_loss: 7.2918
    Epoch 27/60
    5/5 [==============================] - 0s 16ms/step - loss: 6.6627 - val_loss: 8.4363
    Epoch 28/60
    5/5 [==============================] - 0s 14ms/step - loss: 6.5920 - val_loss: 7.3432
    Epoch 29/60
    5/5 [==============================] - 0s 16ms/step - loss: 6.5210 - val_loss: 7.5411
    Epoch 30/60
    5/5 [==============================] - 0s 16ms/step - loss: 6.4248 - val_loss: 7.4086
    Epoch 31/60
    5/5 [==============================] - 0s 16ms/step - loss: 6.3253 - val_loss: 7.2187
    Epoch 32/60
    5/5 [==============================] - 0s 14ms/step - loss: 6.2615 - val_loss: 8.7982
    Epoch 33/60
    5/5 [==============================] - 0s 15ms/step - loss: 6.2840 - val_loss: 6.8902
    Epoch 34/60
    5/5 [==============================] - 0s 15ms/step - loss: 6.3683 - val_loss: 6.9833
    Epoch 35/60
    5/5 [==============================] - 0s 17ms/step - loss: 6.2960 - val_loss: 9.1192
    Epoch 36/60
    5/5 [==============================] - 0s 14ms/step - loss: 5.9451 - val_loss: 5.6797
    Epoch 37/60
    5/5 [==============================] - 0s 14ms/step - loss: 6.0797 - val_loss: 7.3770
    Epoch 38/60
    5/5 [==============================] - 0s 14ms/step - loss: 6.0958 - val_loss: 7.6819
    Epoch 39/60
    5/5 [==============================] - 0s 13ms/step - loss: 5.8846 - val_loss: 5.0449
    Epoch 40/60
    5/5 [==============================] - 0s 14ms/step - loss: 5.7284 - val_loss: 8.1378
    Epoch 41/60
    5/5 [==============================] - 0s 14ms/step - loss: 5.6734 - val_loss: 6.6825
    Epoch 42/60
    5/5 [==============================] - 0s 15ms/step - loss: 5.3407 - val_loss: 5.5715
    Epoch 43/60
    5/5 [==============================] - 0s 15ms/step - loss: 5.2411 - val_loss: 6.5473
    Epoch 44/60
    5/5 [==============================] - 0s 15ms/step - loss: 5.2081 - val_loss: 6.3770
    Epoch 45/60
    5/5 [==============================] - 0s 15ms/step - loss: 4.9366 - val_loss: 5.3922
    Epoch 46/60
    5/5 [==============================] - 0s 15ms/step - loss: 4.8024 - val_loss: 6.9652
    Epoch 47/60
    5/5 [==============================] - 0s 16ms/step - loss: 4.8254 - val_loss: 5.5053
    Epoch 48/60
    5/5 [==============================] - 0s 13ms/step - loss: 4.6412 - val_loss: 5.2221
    Epoch 49/60
    5/5 [==============================] - 0s 14ms/step - loss: 4.4582 - val_loss: 5.5763
    Epoch 50/60
    5/5 [==============================] - 0s 13ms/step - loss: 4.3742 - val_loss: 4.9488
    Epoch 51/60
    5/5 [==============================] - 0s 15ms/step - loss: 4.2366 - val_loss: 5.5124
    Epoch 52/60
    5/5 [==============================] - 0s 16ms/step - loss: 4.1009 - val_loss: 4.1564
    Epoch 53/60
    5/5 [==============================] - 0s 14ms/step - loss: 4.0176 - val_loss: 4.8410
    Epoch 54/60
    5/5 [==============================] - 0s 15ms/step - loss: 3.8634 - val_loss: 4.8028
    Epoch 55/60
    5/5 [==============================] - 0s 15ms/step - loss: 3.6746 - val_loss: 4.9159
    Epoch 56/60
    5/5 [==============================] - 0s 15ms/step - loss: 3.5237 - val_loss: 4.0780
    Epoch 57/60
    5/5 [==============================] - 0s 15ms/step - loss: 3.4468 - val_loss: 4.3971
    Epoch 58/60
    5/5 [==============================] - 0s 15ms/step - loss: 3.3585 - val_loss: 4.3302
    Epoch 59/60
    5/5 [==============================] - 0s 15ms/step - loss: 3.2523 - val_loss: 3.7534
    Epoch 60/60
    5/5 [==============================] - 0s 13ms/step - loss: 3.1345 - val_loss: 3.6678
    Validation Loss for Interval 4:
    [3217.3994140625, 2277.609619140625, 1379.0546875, 570.0361938476562, 71.32405853271484, 48.97214889526367, 148.76214599609375, 64.7107162475586, 13.405189514160156, 23.439857482910156, 25.169750213623047, 12.83476448059082, 7.310492038726807, 11.02135181427002, 11.56486701965332, 9.523015975952148, 8.868061065673828, 8.225914001464844, 7.454861164093018, 8.618672370910645, 8.737471580505371, 8.63959789276123, 8.581700325012207, 7.733956813812256, 7.633740425109863, 7.291750907897949, 8.436331748962402, 7.343202590942383, 7.541126251220703, 7.408626556396484, 7.218733787536621, 8.798218727111816, 6.890194892883301, 6.9832844734191895, 9.119187355041504, 5.679703712463379, 7.3770294189453125, 7.681875705718994, 5.044881343841553, 8.137762069702148, 6.682547092437744, 5.571499824523926, 6.547275543212891, 6.37700080871582, 5.3921990394592285, 6.965160846710205, 5.505305767059326, 5.2220892906188965, 5.576313018798828, 4.9488067626953125, 5.512425422668457, 4.156357288360596, 4.840984344482422, 4.802842617034912, 4.915911674499512, 4.0780181884765625, 4.397127628326416, 4.330187797546387, 3.753401279449463, 3.667808771133423]
    ========================================
    Decoded Forecasts for Interval 4 (Forecast Date: 2009-01-01):
    PRCP: [7.8889456 7.9147673 7.306735  7.676036  7.6748247 7.6759214] (Average: 7.69)
    TAVG: [69.42198  69.65422  66.90076  65.06787  65.267456 65.99384 ] (Average: 67.05)
    TMAX: [81.01787  81.29035  77.59635  76.04901  76.26774  77.068085] (Average: 78.21)
    TMIN: [57.439377 57.660538 55.548073 53.769814 53.95415  54.6224  ] (Average: 55.50)
    ========================================
    Epoch 1/60
    4/4 [==============================] - 1s 84ms/step - loss: 3663.4028 - val_loss: 3276.0320
    Epoch 2/60
    4/4 [==============================] - 0s 20ms/step - loss: 2864.2837 - val_loss: 2525.1943
    Epoch 3/60
    4/4 [==============================] - 0s 20ms/step - loss: 2196.4819 - val_loss: 1896.6510
    Epoch 4/60
    4/4 [==============================] - 0s 19ms/step - loss: 1606.6453 - val_loss: 1296.4220
    Epoch 5/60
    4/4 [==============================] - 0s 19ms/step - loss: 1044.4814 - val_loss: 746.1825
    Epoch 6/60
    4/4 [==============================] - 0s 17ms/step - loss: 553.9184 - val_loss: 327.6507
    Epoch 7/60
    4/4 [==============================] - 0s 18ms/step - loss: 214.0758 - val_loss: 93.0451
    Epoch 8/60
    4/4 [==============================] - 0s 18ms/step - loss: 60.3640 - val_loss: 43.9606
    Epoch 9/60
    4/4 [==============================] - 0s 20ms/step - loss: 51.2836 - val_loss: 74.7561
    Epoch 10/60
    4/4 [==============================] - 0s 20ms/step - loss: 76.5320 - val_loss: 79.3642
    Epoch 11/60
    4/4 [==============================] - 0s 20ms/step - loss: 66.2523 - val_loss: 48.7951
    Epoch 12/60
    4/4 [==============================] - 0s 19ms/step - loss: 34.4626 - val_loss: 21.3124
    Epoch 13/60
    4/4 [==============================] - 0s 18ms/step - loss: 13.4102 - val_loss: 11.5654
    Epoch 14/60
    4/4 [==============================] - 0s 17ms/step - loss: 10.4480 - val_loss: 13.4577
    Epoch 15/60
    4/4 [==============================] - 0s 20ms/step - loss: 13.5951 - val_loss: 14.8496
    Epoch 16/60
    4/4 [==============================] - 0s 21ms/step - loss: 13.1514 - val_loss: 11.4077
    Epoch 17/60
    4/4 [==============================] - 0s 21ms/step - loss: 9.3733 - val_loss: 8.0193
    Epoch 18/60
    4/4 [==============================] - 0s 21ms/step - loss: 6.6894 - val_loss: 7.2845
    Epoch 19/60
    4/4 [==============================] - 0s 21ms/step - loss: 6.5427 - val_loss: 7.4663
    Epoch 20/60
    4/4 [==============================] - 0s 29ms/step - loss: 7.0107 - val_loss: 7.1503
    Epoch 21/60
    4/4 [==============================] - 0s 19ms/step - loss: 6.8636 - val_loss: 7.0687
    Epoch 22/60
    4/4 [==============================] - 0s 21ms/step - loss: 6.4002 - val_loss: 7.1790
    Epoch 23/60
    4/4 [==============================] - 0s 18ms/step - loss: 6.0740 - val_loss: 6.4700
    Epoch 24/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.9962 - val_loss: 6.4432
    Epoch 25/60
    4/4 [==============================] - 0s 17ms/step - loss: 6.0141 - val_loss: 6.4744
    Epoch 26/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.9334 - val_loss: 6.0813
    Epoch 27/60
    4/4 [==============================] - 0s 20ms/step - loss: 5.8254 - val_loss: 6.1067
    Epoch 28/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.7140 - val_loss: 6.3424
    Epoch 29/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.6799 - val_loss: 6.3775
    Epoch 30/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.6746 - val_loss: 6.1164
    Epoch 31/60
    4/4 [==============================] - 0s 20ms/step - loss: 5.5686 - val_loss: 5.7586
    Epoch 32/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.4864 - val_loss: 5.7723
    Epoch 33/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.4397 - val_loss: 5.8269
    Epoch 34/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.3607 - val_loss: 5.5466
    Epoch 35/60
    4/4 [==============================] - 0s 20ms/step - loss: 5.3280 - val_loss: 5.6332
    Epoch 36/60
    4/4 [==============================] - 0s 21ms/step - loss: 5.2171 - val_loss: 5.0447
    Epoch 37/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.1049 - val_loss: 5.2198
    Epoch 38/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.0330 - val_loss: 5.0308
    Epoch 39/60
    4/4 [==============================] - 0s 17ms/step - loss: 4.9074 - val_loss: 4.5967
    Epoch 40/60
    4/4 [==============================] - 0s 19ms/step - loss: 4.8162 - val_loss: 4.6012
    Epoch 41/60
    4/4 [==============================] - 0s 20ms/step - loss: 4.6946 - val_loss: 4.9535
    Epoch 42/60
    4/4 [==============================] - 0s 17ms/step - loss: 4.6179 - val_loss: 4.6637
    Epoch 43/60
    4/4 [==============================] - 0s 20ms/step - loss: 4.4592 - val_loss: 4.1409
    Epoch 44/60
    4/4 [==============================] - 0s 20ms/step - loss: 4.3355 - val_loss: 4.0688
    Epoch 45/60
    4/4 [==============================] - 0s 19ms/step - loss: 4.2013 - val_loss: 4.1735
    Epoch 46/60
    4/4 [==============================] - 0s 20ms/step - loss: 4.1347 - val_loss: 4.2835
    Epoch 47/60
    4/4 [==============================] - 0s 18ms/step - loss: 4.0488 - val_loss: 3.7793
    Epoch 48/60
    4/4 [==============================] - 0s 17ms/step - loss: 3.9058 - val_loss: 3.9843
    Epoch 49/60
    4/4 [==============================] - 0s 18ms/step - loss: 3.8465 - val_loss: 3.8599
    Epoch 50/60
    4/4 [==============================] - 0s 18ms/step - loss: 3.7554 - val_loss: 3.6264
    Epoch 51/60
    4/4 [==============================] - 0s 17ms/step - loss: 3.6537 - val_loss: 3.3055
    Epoch 52/60
    4/4 [==============================] - 0s 20ms/step - loss: 3.5317 - val_loss: 3.4228
    Epoch 53/60
    4/4 [==============================] - 0s 16ms/step - loss: 3.4262 - val_loss: 3.3563
    Epoch 54/60
    4/4 [==============================] - 0s 19ms/step - loss: 3.3077 - val_loss: 3.1730
    Epoch 55/60
    4/4 [==============================] - 0s 17ms/step - loss: 3.1858 - val_loss: 3.1657
    Epoch 56/60
    4/4 [==============================] - 0s 20ms/step - loss: 3.0996 - val_loss: 2.8585
    Epoch 57/60
    4/4 [==============================] - 0s 19ms/step - loss: 2.9869 - val_loss: 2.9284
    Epoch 58/60
    4/4 [==============================] - 0s 21ms/step - loss: 2.9060 - val_loss: 2.6932
    Epoch 59/60
    4/4 [==============================] - 0s 20ms/step - loss: 2.8439 - val_loss: 2.5856
    Epoch 60/60
    4/4 [==============================] - 0s 18ms/step - loss: 2.7513 - val_loss: 2.4231
    Validation Loss for Interval 5:
    [3276.031982421875, 2525.1943359375, 1896.6510009765625, 1296.4219970703125, 746.1824951171875, 327.65069580078125, 93.04510498046875, 43.96056365966797, 74.75605010986328, 79.36424255371094, 48.795074462890625, 21.312440872192383, 11.565446853637695, 13.457718849182129, 14.849567413330078, 11.407651901245117, 8.019316673278809, 7.284513473510742, 7.466320991516113, 7.150327205657959, 7.068691730499268, 7.179008483886719, 6.469976425170898, 6.443163871765137, 6.474407196044922, 6.08128547668457, 6.106719017028809, 6.342400550842285, 6.377500057220459, 6.116388320922852, 5.758619785308838, 5.77230978012085, 5.826878547668457, 5.5466084480285645, 5.6332478523254395, 5.044732570648193, 5.2198052406311035, 5.030832290649414, 4.59666109085083, 4.6011810302734375, 4.953503131866455, 4.6636528968811035, 4.140872955322266, 4.06878137588501, 4.173481464385986, 4.2834954261779785, 3.779262065887451, 3.984253406524658, 3.8598506450653076, 3.626434564590454, 3.3055267333984375, 3.4227795600891113, 3.356323719024658, 3.1729843616485596, 3.1657207012176514, 2.8585257530212402, 2.9283533096313477, 2.6931698322296143, 2.5855813026428223, 2.423062562942505]
    ========================================
    Decoded Forecasts for Interval 5 (Forecast Date: 2010-01-01):
    PRCP: [8.733152 8.68619  8.654968 8.475517] (Average: 8.64)
    TAVG: [66.57971 70.68227 70.47765 69.15205] (Average: 69.22)
    TMAX: [75.99742  80.81039  80.62097  79.345634] (Average: 79.19)
    TMIN: [55.649548 58.72917  58.538643 57.307407] (Average: 57.56)
    ========================================
    Epoch 1/60
    4/4 [==============================] - 1s 76ms/step - loss: 2023.9136 - val_loss: 1553.4941
    Epoch 2/60
    4/4 [==============================] - 0s 28ms/step - loss: 1226.8989 - val_loss: 814.2997
    Epoch 3/60
    4/4 [==============================] - 0s 16ms/step - loss: 586.6083 - val_loss: 279.8893
    Epoch 4/60
    4/4 [==============================] - 0s 16ms/step - loss: 170.1696 - val_loss: 34.9433
    Epoch 5/60
    4/4 [==============================] - 0s 18ms/step - loss: 38.2710 - val_loss: 67.4864
    Epoch 6/60
    4/4 [==============================] - 0s 17ms/step - loss: 89.1832 - val_loss: 122.7308
    Epoch 7/60
    4/4 [==============================] - 0s 18ms/step - loss: 100.9274 - val_loss: 83.0338
    Epoch 8/60
    4/4 [==============================] - 0s 17ms/step - loss: 51.4903 - val_loss: 30.6330
    Epoch 9/60
    4/4 [==============================] - 0s 19ms/step - loss: 17.7077 - val_loss: 15.8403
    Epoch 10/60
    4/4 [==============================] - 0s 18ms/step - loss: 15.5625 - val_loss: 19.7244
    Epoch 11/60
    4/4 [==============================] - 0s 16ms/step - loss: 19.9085 - val_loss: 19.3638
    Epoch 12/60
    4/4 [==============================] - 0s 18ms/step - loss: 17.6878 - val_loss: 13.6163
    Epoch 13/60
    4/4 [==============================] - 0s 17ms/step - loss: 12.0666 - val_loss: 8.9601
    Epoch 14/60
    4/4 [==============================] - 0s 18ms/step - loss: 8.6600 - val_loss: 8.2447
    Epoch 15/60
    4/4 [==============================] - 0s 16ms/step - loss: 8.2810 - val_loss: 9.1452
    Epoch 16/60
    4/4 [==============================] - 0s 19ms/step - loss: 8.3975 - val_loss: 9.6226
    Epoch 17/60
    4/4 [==============================] - 0s 18ms/step - loss: 7.7180 - val_loss: 9.0311
    Epoch 18/60
    4/4 [==============================] - 0s 16ms/step - loss: 6.8310 - val_loss: 7.6818
    Epoch 19/60
    4/4 [==============================] - 0s 17ms/step - loss: 6.3511 - val_loss: 7.4284
    Epoch 20/60
    4/4 [==============================] - 0s 18ms/step - loss: 6.4155 - val_loss: 6.6750
    Epoch 21/60
    4/4 [==============================] - 0s 19ms/step - loss: 6.3209 - val_loss: 6.2222
    Epoch 22/60
    4/4 [==============================] - 0s 17ms/step - loss: 6.0259 - val_loss: 6.3362
    Epoch 23/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.8534 - val_loss: 6.9486
    Epoch 24/60
    4/4 [==============================] - 0s 28ms/step - loss: 5.8064 - val_loss: 7.1915
    Epoch 25/60
    4/4 [==============================] - 0s 16ms/step - loss: 5.7886 - val_loss: 6.4276
    Epoch 26/60
    4/4 [==============================] - 0s 16ms/step - loss: 5.6137 - val_loss: 6.1056
    Epoch 27/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.5168 - val_loss: 5.8589
    Epoch 28/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.4664 - val_loss: 5.6897
    Epoch 29/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.3229 - val_loss: 6.0386
    Epoch 30/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.2504 - val_loss: 5.7552
    Epoch 31/60
    4/4 [==============================] - 0s 16ms/step - loss: 5.0920 - val_loss: 5.5920
    Epoch 32/60
    4/4 [==============================] - 0s 17ms/step - loss: 4.9371 - val_loss: 5.3226
    Epoch 33/60
    4/4 [==============================] - 0s 16ms/step - loss: 4.7794 - val_loss: 4.8074
    Epoch 34/60
    4/4 [==============================] - 0s 16ms/step - loss: 4.6186 - val_loss: 4.8965
    Epoch 35/60
    4/4 [==============================] - 0s 18ms/step - loss: 4.5152 - val_loss: 5.2269
    Epoch 36/60
    4/4 [==============================] - 0s 16ms/step - loss: 4.3998 - val_loss: 4.7014
    Epoch 37/60
    4/4 [==============================] - 0s 17ms/step - loss: 4.2896 - val_loss: 4.5028
    Epoch 38/60
    4/4 [==============================] - 0s 16ms/step - loss: 4.1961 - val_loss: 4.4793
    Epoch 39/60
    4/4 [==============================] - 0s 16ms/step - loss: 4.0497 - val_loss: 4.2002
    Epoch 40/60
    4/4 [==============================] - 0s 17ms/step - loss: 4.0206 - val_loss: 3.9949
    Epoch 41/60
    4/4 [==============================] - 0s 18ms/step - loss: 3.8427 - val_loss: 4.0380
    Epoch 42/60
    4/4 [==============================] - 0s 16ms/step - loss: 3.7499 - val_loss: 3.9557
    Epoch 43/60
    4/4 [==============================] - 0s 19ms/step - loss: 3.6036 - val_loss: 3.5733
    Epoch 44/60
    4/4 [==============================] - 0s 18ms/step - loss: 3.5051 - val_loss: 3.0932
    Epoch 45/60
    4/4 [==============================] - 0s 17ms/step - loss: 3.4146 - val_loss: 3.2980
    Epoch 46/60
    4/4 [==============================] - 0s 18ms/step - loss: 3.2695 - val_loss: 3.2637
    Epoch 47/60
    4/4 [==============================] - 0s 16ms/step - loss: 3.1709 - val_loss: 2.8755
    Epoch 48/60
    4/4 [==============================] - 0s 19ms/step - loss: 3.0783 - val_loss: 2.6382
    Epoch 49/60
    4/4 [==============================] - 0s 16ms/step - loss: 2.9430 - val_loss: 3.0054
    Epoch 50/60
    4/4 [==============================] - 0s 16ms/step - loss: 2.8587 - val_loss: 2.3902
    Epoch 51/60
    4/4 [==============================] - 0s 16ms/step - loss: 2.7458 - val_loss: 2.3149
    Epoch 52/60
    4/4 [==============================] - 0s 16ms/step - loss: 2.6715 - val_loss: 2.2312
    Epoch 53/60
    4/4 [==============================] - 0s 18ms/step - loss: 2.5405 - val_loss: 2.0086
    Epoch 54/60
    4/4 [==============================] - 0s 17ms/step - loss: 2.4491 - val_loss: 1.9549
    Epoch 55/60
    4/4 [==============================] - 0s 18ms/step - loss: 2.3795 - val_loss: 1.9286
    Epoch 56/60
    4/4 [==============================] - 0s 16ms/step - loss: 2.2794 - val_loss: 1.7265
    Epoch 57/60
    4/4 [==============================] - 0s 17ms/step - loss: 2.2364 - val_loss: 1.6778
    Epoch 58/60
    4/4 [==============================] - 0s 17ms/step - loss: 2.1898 - val_loss: 1.5666
    Epoch 59/60
    4/4 [==============================] - 0s 17ms/step - loss: 2.0917 - val_loss: 1.3999
    Epoch 60/60
    4/4 [==============================] - 0s 15ms/step - loss: 2.0482 - val_loss: 1.3745
    Validation Loss for Interval 6:
    [1553.494140625, 814.2997436523438, 279.8892822265625, 34.943321228027344, 67.48637390136719, 122.7308120727539, 83.03375244140625, 30.632972717285156, 15.840265274047852, 19.72439956665039, 19.363805770874023, 13.616323471069336, 8.960076332092285, 8.244688034057617, 9.145221710205078, 9.622604370117188, 9.03105640411377, 7.681835174560547, 7.428386688232422, 6.675036907196045, 6.222222328186035, 6.336245059967041, 6.948636054992676, 7.191530704498291, 6.4275689125061035, 6.105567455291748, 5.858889579772949, 5.689702987670898, 6.03856086730957, 5.755178451538086, 5.592011451721191, 5.32255220413208, 4.807358741760254, 4.896528244018555, 5.226916313171387, 4.701371192932129, 4.502846717834473, 4.479312419891357, 4.2001543045043945, 3.994877576828003, 4.037958145141602, 3.955728054046631, 3.573315382003784, 3.093204975128174, 3.2979700565338135, 3.263652801513672, 2.875504970550537, 2.638239622116089, 3.005387783050537, 2.390230417251587, 2.314889430999756, 2.2312161922454834, 2.0085506439208984, 1.954934000968933, 1.9286096096038818, 1.7264854907989502, 1.6777522563934326, 1.5666351318359375, 1.3999427556991577, 1.374455451965332]
    ========================================
    Decoded Forecasts for Interval 6 (Forecast Date: 2011-01-01):
    PRCP: [9.046675 8.941927 8.751043] (Average: 8.91)
    TAVG: [70.34316  70.684784 70.13954 ] (Average: 70.39)
    TMAX: [80.93307  81.09934  79.792656] (Average: 80.61)
    TMIN: [57.448803 58.196644 57.79394 ] (Average: 57.81)
    ========================================
    Epoch 1/60
    4/4 [==============================] - 1s 81ms/step - loss: 3730.9431 - val_loss: 3463.1021
    Epoch 2/60
    4/4 [==============================] - 0s 17ms/step - loss: 3101.9258 - val_loss: 2912.7510
    Epoch 3/60
    4/4 [==============================] - 0s 21ms/step - loss: 2585.8906 - val_loss: 2388.6729
    Epoch 4/60
    4/4 [==============================] - 0s 19ms/step - loss: 2066.4143 - val_loss: 1788.3724
    Epoch 5/60
    4/4 [==============================] - 0s 28ms/step - loss: 1464.2766 - val_loss: 1127.9274
    Epoch 6/60
    4/4 [==============================] - 0s 17ms/step - loss: 842.0726 - val_loss: 508.6673
    Epoch 7/60
    4/4 [==============================] - 0s 18ms/step - loss: 318.3524 - val_loss: 105.2604
    Epoch 8/60
    4/4 [==============================] - 0s 18ms/step - loss: 56.2645 - val_loss: 41.6047
    Epoch 9/60
    4/4 [==============================] - 0s 19ms/step - loss: 86.5981 - val_loss: 132.9996
    Epoch 10/60
    4/4 [==============================] - 0s 18ms/step - loss: 146.3794 - val_loss: 111.0267
    Epoch 11/60
    4/4 [==============================] - 0s 17ms/step - loss: 90.5818 - val_loss: 43.3160
    Epoch 12/60
    4/4 [==============================] - 0s 20ms/step - loss: 30.3048 - val_loss: 26.7736
    Epoch 13/60
    4/4 [==============================] - 0s 18ms/step - loss: 19.6516 - val_loss: 38.7351
    Epoch 14/60
    4/4 [==============================] - 0s 16ms/step - loss: 27.1448 - val_loss: 39.7872
    Epoch 15/60
    4/4 [==============================] - 0s 17ms/step - loss: 24.7969 - val_loss: 26.0442
    Epoch 16/60
    4/4 [==============================] - 0s 19ms/step - loss: 15.5742 - val_loss: 11.8497
    Epoch 17/60
    4/4 [==============================] - 0s 19ms/step - loss: 10.4638 - val_loss: 6.4307
    Epoch 18/60
    4/4 [==============================] - 0s 20ms/step - loss: 10.5030 - val_loss: 6.5052
    Epoch 19/60
    4/4 [==============================] - 0s 21ms/step - loss: 10.4821 - val_loss: 7.4844
    Epoch 20/60
    4/4 [==============================] - 0s 20ms/step - loss: 8.9531 - val_loss: 9.5190
    Epoch 21/60
    4/4 [==============================] - 0s 18ms/step - loss: 8.0553 - val_loss: 11.6662
    Epoch 22/60
    4/4 [==============================] - 0s 17ms/step - loss: 8.1838 - val_loss: 12.5078
    Epoch 23/60
    4/4 [==============================] - 0s 19ms/step - loss: 8.0811 - val_loss: 10.8929
    Epoch 24/60
    4/4 [==============================] - 0s 19ms/step - loss: 7.6344 - val_loss: 8.7693
    Epoch 25/60
    4/4 [==============================] - 0s 17ms/step - loss: 7.4475 - val_loss: 7.1205
    Epoch 26/60
    4/4 [==============================] - 0s 19ms/step - loss: 7.5144 - val_loss: 6.9386
    Epoch 27/60
    4/4 [==============================] - 0s 19ms/step - loss: 7.5108 - val_loss: 7.8510
    Epoch 28/60
    4/4 [==============================] - 0s 29ms/step - loss: 7.3541 - val_loss: 8.8944
    Epoch 29/60
    4/4 [==============================] - 0s 18ms/step - loss: 7.2862 - val_loss: 9.1760
    Epoch 30/60
    4/4 [==============================] - 0s 18ms/step - loss: 7.2659 - val_loss: 8.9050
    Epoch 31/60
    4/4 [==============================] - 0s 17ms/step - loss: 7.2326 - val_loss: 8.4583
    Epoch 32/60
    4/4 [==============================] - 0s 19ms/step - loss: 7.1657 - val_loss: 7.7851
    Epoch 33/60
    4/4 [==============================] - 0s 19ms/step - loss: 7.1376 - val_loss: 7.4839
    Epoch 34/60
    4/4 [==============================] - 0s 19ms/step - loss: 7.1339 - val_loss: 7.6212
    Epoch 35/60
    4/4 [==============================] - 0s 19ms/step - loss: 7.0518 - val_loss: 8.5834
    Epoch 36/60
    4/4 [==============================] - 0s 19ms/step - loss: 7.0853 - val_loss: 8.7088
    Epoch 37/60
    4/4 [==============================] - 0s 19ms/step - loss: 7.0058 - val_loss: 7.9908
    Epoch 38/60
    4/4 [==============================] - 0s 20ms/step - loss: 6.9612 - val_loss: 7.6883
    Epoch 39/60
    4/4 [==============================] - 0s 19ms/step - loss: 6.9535 - val_loss: 7.7700
    Epoch 40/60
    4/4 [==============================] - 0s 20ms/step - loss: 6.8698 - val_loss: 8.6711
    Epoch 41/60
    4/4 [==============================] - 0s 19ms/step - loss: 6.8325 - val_loss: 8.2461
    Epoch 42/60
    4/4 [==============================] - 0s 19ms/step - loss: 6.7397 - val_loss: 8.0167
    Epoch 43/60
    4/4 [==============================] - 0s 18ms/step - loss: 6.7070 - val_loss: 7.2829
    Epoch 44/60
    4/4 [==============================] - 0s 19ms/step - loss: 6.6999 - val_loss: 7.0615
    Epoch 45/60
    4/4 [==============================] - 0s 19ms/step - loss: 6.6562 - val_loss: 7.3945
    Epoch 46/60
    4/4 [==============================] - 0s 19ms/step - loss: 6.6130 - val_loss: 8.1179
    Epoch 47/60
    4/4 [==============================] - 0s 19ms/step - loss: 6.6121 - val_loss: 7.8067
    Epoch 48/60
    4/4 [==============================] - 0s 18ms/step - loss: 6.5420 - val_loss: 7.7873
    Epoch 49/60
    4/4 [==============================] - 0s 20ms/step - loss: 6.4995 - val_loss: 7.6735
    Epoch 50/60
    4/4 [==============================] - 0s 20ms/step - loss: 6.5113 - val_loss: 6.9694
    Epoch 51/60
    4/4 [==============================] - 0s 19ms/step - loss: 6.4500 - val_loss: 6.9991
    Epoch 52/60
    4/4 [==============================] - 0s 21ms/step - loss: 6.3806 - val_loss: 7.6021
    Epoch 53/60
    4/4 [==============================] - 0s 21ms/step - loss: 6.3685 - val_loss: 7.9115
    Epoch 54/60
    4/4 [==============================] - 0s 21ms/step - loss: 6.3474 - val_loss: 7.5309
    Epoch 55/60
    4/4 [==============================] - 0s 18ms/step - loss: 6.2707 - val_loss: 6.6467
    Epoch 56/60
    4/4 [==============================] - 0s 18ms/step - loss: 6.2337 - val_loss: 6.5221
    Epoch 57/60
    4/4 [==============================] - 0s 17ms/step - loss: 6.1917 - val_loss: 6.6446
    Epoch 58/60
    4/4 [==============================] - 0s 18ms/step - loss: 6.1351 - val_loss: 7.1161
    Epoch 59/60
    4/4 [==============================] - 0s 17ms/step - loss: 6.0991 - val_loss: 6.6912
    Epoch 60/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.9999 - val_loss: 6.8313
    Validation Loss for Interval 7:
    [3463.10205078125, 2912.7509765625, 2388.6728515625, 1788.3724365234375, 1127.9273681640625, 508.6672668457031, 105.26041412353516, 41.60466384887695, 132.99957275390625, 111.02672576904297, 43.31599044799805, 26.773624420166016, 38.73514938354492, 39.787227630615234, 26.044231414794922, 11.8496675491333, 6.43072509765625, 6.505205154418945, 7.48444938659668, 9.51904296875, 11.66617202758789, 12.507767677307129, 10.892918586730957, 8.769251823425293, 7.120519161224365, 6.938593864440918, 7.85100793838501, 8.894378662109375, 9.175997734069824, 8.904955863952637, 8.45827865600586, 7.785143852233887, 7.483915328979492, 7.621176242828369, 8.583430290222168, 8.708834648132324, 7.990781784057617, 7.688261032104492, 7.770037651062012, 8.671100616455078, 8.246106147766113, 8.016730308532715, 7.282933712005615, 7.061519145965576, 7.3945159912109375, 8.117939949035645, 7.806683540344238, 7.7873215675354, 7.6734538078308105, 6.969411373138428, 6.999093532562256, 7.602070331573486, 7.911452293395996, 7.530903339385986, 6.646749496459961, 6.5221123695373535, 6.644609451293945, 7.116089820861816, 6.691167831420898, 6.831295490264893]
    ========================================
    Decoded Forecasts for Interval 7 (Forecast Date: 2012-01-01):
    PRCP: [4.5986533 4.683843  4.4650035 4.504395 ] (Average: 4.56)
    TAVG: [68.858765 68.32321  69.650024 69.56952 ] (Average: 69.10)
    TMAX: [79.901825 79.15927  81.025856 80.86925 ] (Average: 80.24)
    TMIN: [56.491535 56.05479  57.13601  57.040188] (Average: 56.68)
    ========================================
    Epoch 1/60
    4/4 [==============================] - 1s 82ms/step - loss: 3491.3057 - val_loss: 3068.5308
    Epoch 2/60
    4/4 [==============================] - 0s 20ms/step - loss: 2698.4324 - val_loss: 2282.4131
    Epoch 3/60
    4/4 [==============================] - 0s 18ms/step - loss: 1979.7061 - val_loss: 1585.9716
    Epoch 4/60
    4/4 [==============================] - 0s 21ms/step - loss: 1296.1011 - val_loss: 898.8517
    Epoch 5/60
    4/4 [==============================] - 0s 18ms/step - loss: 665.6084 - val_loss: 357.4142
    Epoch 6/60
    4/4 [==============================] - 0s 18ms/step - loss: 210.5032 - val_loss: 86.0622
    Epoch 7/60
    4/4 [==============================] - 0s 17ms/step - loss: 43.5153 - val_loss: 93.5740
    Epoch 8/60
    4/4 [==============================] - 0s 19ms/step - loss: 96.7341 - val_loss: 137.2985
    Epoch 9/60
    4/4 [==============================] - 0s 17ms/step - loss: 121.6773 - val_loss: 76.5023
    Epoch 10/60
    4/4 [==============================] - 0s 28ms/step - loss: 65.6567 - val_loss: 17.5880
    Epoch 11/60
    4/4 [==============================] - 0s 17ms/step - loss: 25.5778 - val_loss: 10.1127
    Epoch 12/60
    4/4 [==============================] - 0s 19ms/step - loss: 19.5085 - val_loss: 20.7279
    Epoch 13/60
    4/4 [==============================] - 0s 18ms/step - loss: 19.7286 - val_loss: 27.5453
    Epoch 14/60
    4/4 [==============================] - 0s 16ms/step - loss: 17.4692 - val_loss: 29.8380
    Epoch 15/60
    4/4 [==============================] - 0s 17ms/step - loss: 14.3206 - val_loss: 25.9953
    Epoch 16/60
    4/4 [==============================] - 0s 19ms/step - loss: 10.8797 - val_loss: 17.1564
    Epoch 17/60
    4/4 [==============================] - 0s 18ms/step - loss: 7.7821 - val_loss: 9.2832
    Epoch 18/60
    4/4 [==============================] - 0s 17ms/step - loss: 7.2046 - val_loss: 6.0946
    Epoch 19/60
    4/4 [==============================] - 0s 19ms/step - loss: 8.0027 - val_loss: 5.8126
    Epoch 20/60
    4/4 [==============================] - 0s 17ms/step - loss: 7.5651 - val_loss: 6.8896
    Epoch 21/60
    4/4 [==============================] - 0s 16ms/step - loss: 6.4939 - val_loss: 9.3643
    Epoch 22/60
    4/4 [==============================] - 0s 17ms/step - loss: 6.3204 - val_loss: 11.8632
    Epoch 23/60
    4/4 [==============================] - 0s 18ms/step - loss: 6.5303 - val_loss: 12.0313
    Epoch 24/60
    4/4 [==============================] - 0s 16ms/step - loss: 6.4464 - val_loss: 10.8383
    Epoch 25/60
    4/4 [==============================] - 0s 19ms/step - loss: 6.2106 - val_loss: 9.4854
    Epoch 26/60
    4/4 [==============================] - 0s 17ms/step - loss: 6.0789 - val_loss: 8.6478
    Epoch 27/60
    4/4 [==============================] - 0s 16ms/step - loss: 6.1014 - val_loss: 8.0187
    Epoch 28/60
    4/4 [==============================] - 0s 18ms/step - loss: 6.0297 - val_loss: 8.5957
    Epoch 29/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.9808 - val_loss: 9.8046
    Epoch 30/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.9501 - val_loss: 9.4824
    Epoch 31/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.8563 - val_loss: 8.3485
    Epoch 32/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.8435 - val_loss: 8.4704
    Epoch 33/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.7696 - val_loss: 8.7616
    Epoch 34/60
    4/4 [==============================] - 0s 28ms/step - loss: 5.7436 - val_loss: 8.3560
    Epoch 35/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.6870 - val_loss: 7.7577
    Epoch 36/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.6550 - val_loss: 7.6686
    Epoch 37/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.5678 - val_loss: 8.2153
    Epoch 38/60
    4/4 [==============================] - 0s 20ms/step - loss: 5.5673 - val_loss: 8.6394
    Epoch 39/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.5560 - val_loss: 8.2295
    Epoch 40/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.4527 - val_loss: 7.9878
    Epoch 41/60
    4/4 [==============================] - 0s 20ms/step - loss: 5.4403 - val_loss: 7.9224
    Epoch 42/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.3876 - val_loss: 7.5817
    Epoch 43/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.3238 - val_loss: 7.5138
    Epoch 44/60
    4/4 [==============================] - 0s 16ms/step - loss: 5.2953 - val_loss: 7.5307
    Epoch 45/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.2463 - val_loss: 7.3515
    Epoch 46/60
    4/4 [==============================] - 0s 16ms/step - loss: 5.1941 - val_loss: 7.3534
    Epoch 47/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.1577 - val_loss: 7.2461
    Epoch 48/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.1190 - val_loss: 7.4986
    Epoch 49/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.1040 - val_loss: 7.3703
    Epoch 50/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.0655 - val_loss: 7.2544
    Epoch 51/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.0247 - val_loss: 6.8510
    Epoch 52/60
    4/4 [==============================] - 0s 16ms/step - loss: 4.9918 - val_loss: 6.9861
    Epoch 53/60
    4/4 [==============================] - 0s 19ms/step - loss: 4.9503 - val_loss: 6.7509
    Epoch 54/60
    4/4 [==============================] - 0s 17ms/step - loss: 4.9025 - val_loss: 6.6714
    Epoch 55/60
    4/4 [==============================] - 0s 19ms/step - loss: 4.8786 - val_loss: 6.6041
    Epoch 56/60
    4/4 [==============================] - 0s 19ms/step - loss: 4.8282 - val_loss: 6.6914
    Epoch 57/60
    4/4 [==============================] - 0s 17ms/step - loss: 4.7775 - val_loss: 6.7884
    Epoch 58/60
    4/4 [==============================] - 0s 17ms/step - loss: 4.7396 - val_loss: 6.5398
    Epoch 59/60
    4/4 [==============================] - 0s 18ms/step - loss: 4.7126 - val_loss: 6.4064
    Epoch 60/60
    4/4 [==============================] - 0s 18ms/step - loss: 4.6383 - val_loss: 6.0820
    Validation Loss for Interval 8:
    [3068.53076171875, 2282.4130859375, 1585.9715576171875, 898.8516845703125, 357.4142150878906, 86.06220245361328, 93.57395935058594, 137.2985076904297, 76.5022964477539, 17.587980270385742, 10.112675666809082, 20.727880477905273, 27.54532241821289, 29.837953567504883, 25.995336532592773, 17.156370162963867, 9.283220291137695, 6.094571590423584, 5.812564373016357, 6.889640808105469, 9.364259719848633, 11.863248825073242, 12.031304359436035, 10.838309288024902, 9.485445022583008, 8.647818565368652, 8.018702507019043, 8.595702171325684, 9.804563522338867, 9.482416152954102, 8.348517417907715, 8.470429420471191, 8.761624336242676, 8.35604190826416, 7.7576985359191895, 7.668564796447754, 8.215336799621582, 8.639409065246582, 8.229491233825684, 7.987840175628662, 7.922444820404053, 7.581718444824219, 7.513754844665527, 7.530725955963135, 7.3514838218688965, 7.353447914123535, 7.246100425720215, 7.4985551834106445, 7.3702898025512695, 7.254386901855469, 6.851048946380615, 6.986135959625244, 6.750853538513184, 6.671437740325928, 6.6041412353515625, 6.6913557052612305, 6.78841495513916, 6.539752960205078, 6.406361103057861, 6.082042217254639]
    ========================================
    Decoded Forecasts for Interval 8 (Forecast Date: 2013-01-01):
    PRCP: [5.431483] (Average: 5.43)
    TAVG: [68.46142] (Average: 68.46)
    TMAX: [80.73082] (Average: 80.73)
    TMIN: [57.146576] (Average: 57.15)
    ========================================
    Epoch 1/60
    4/4 [==============================] - 1s 80ms/step - loss: 3436.7388 - val_loss: 2858.6387
    Epoch 2/60
    4/4 [==============================] - 0s 20ms/step - loss: 2591.6040 - val_loss: 2087.5393
    Epoch 3/60
    4/4 [==============================] - 0s 18ms/step - loss: 1874.2822 - val_loss: 1367.8727
    Epoch 4/60
    4/4 [==============================] - 0s 17ms/step - loss: 1190.7589 - val_loss: 713.2156
    Epoch 5/60
    4/4 [==============================] - 0s 19ms/step - loss: 580.6678 - val_loss: 210.7242
    Epoch 6/60
    4/4 [==============================] - 0s 19ms/step - loss: 147.6241 - val_loss: 20.2552
    Epoch 7/60
    4/4 [==============================] - 0s 17ms/step - loss: 25.3218 - val_loss: 125.6146
    Epoch 8/60
    4/4 [==============================] - 0s 18ms/step - loss: 112.7651 - val_loss: 197.4170
    Epoch 9/60
    4/4 [==============================] - 0s 19ms/step - loss: 129.9911 - val_loss: 110.3521
    Epoch 10/60
    4/4 [==============================] - 0s 26ms/step - loss: 55.2412 - val_loss: 27.4438
    Epoch 11/60
    4/4 [==============================] - 0s 18ms/step - loss: 12.7003 - val_loss: 12.2372
    Epoch 12/60
    4/4 [==============================] - 0s 16ms/step - loss: 17.0452 - val_loss: 22.5133
    Epoch 13/60
    4/4 [==============================] - 0s 17ms/step - loss: 25.8301 - val_loss: 23.5583
    Epoch 14/60
    4/4 [==============================] - 0s 20ms/step - loss: 20.8464 - val_loss: 16.5407
    Epoch 15/60
    4/4 [==============================] - 0s 19ms/step - loss: 10.7587 - val_loss: 13.7403
    Epoch 16/60
    4/4 [==============================] - 0s 18ms/step - loss: 7.2311 - val_loss: 16.8360
    Epoch 17/60
    4/4 [==============================] - 0s 18ms/step - loss: 8.7350 - val_loss: 17.8803
    Epoch 18/60
    4/4 [==============================] - 0s 17ms/step - loss: 8.8213 - val_loss: 16.2487
    Epoch 19/60
    4/4 [==============================] - 0s 20ms/step - loss: 6.9661 - val_loss: 13.2997
    Epoch 20/60
    4/4 [==============================] - 0s 18ms/step - loss: 6.0945 - val_loss: 12.1221
    Epoch 21/60
    4/4 [==============================] - 0s 18ms/step - loss: 6.3701 - val_loss: 11.5849
    Epoch 22/60
    4/4 [==============================] - 0s 18ms/step - loss: 6.3574 - val_loss: 11.0495
    Epoch 23/60
    4/4 [==============================] - 0s 17ms/step - loss: 6.0259 - val_loss: 10.8163
    Epoch 24/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.8569 - val_loss: 12.1455
    Epoch 25/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.8949 - val_loss: 13.7819
    Epoch 26/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.9175 - val_loss: 13.1310
    Epoch 27/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.8032 - val_loss: 12.2906
    Epoch 28/60
    4/4 [==============================] - 0s 16ms/step - loss: 5.7139 - val_loss: 11.2162
    Epoch 29/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.7666 - val_loss: 10.7146
    Epoch 30/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.7309 - val_loss: 11.9890
    Epoch 31/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.6339 - val_loss: 11.5734
    Epoch 32/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.5278 - val_loss: 11.1386
    Epoch 33/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.5671 - val_loss: 11.8453
    Epoch 34/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.5428 - val_loss: 11.8896
    Epoch 35/60
    4/4 [==============================] - 0s 21ms/step - loss: 5.4699 - val_loss: 10.5918
    Epoch 36/60
    4/4 [==============================] - 0s 16ms/step - loss: 5.4296 - val_loss: 10.7317
    Epoch 37/60
    4/4 [==============================] - 0s 23ms/step - loss: 5.4161 - val_loss: 10.7951
    Epoch 38/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.3766 - val_loss: 11.8187
    Epoch 39/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.4162 - val_loss: 12.1729
    Epoch 40/60
    4/4 [==============================] - 0s 16ms/step - loss: 5.3578 - val_loss: 11.5656
    Epoch 41/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.2730 - val_loss: 9.9448
    Epoch 42/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.3035 - val_loss: 9.5171
    Epoch 43/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.2202 - val_loss: 11.1531
    Epoch 44/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.2288 - val_loss: 11.4280
    Epoch 45/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.2245 - val_loss: 10.0061
    Epoch 46/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.1765 - val_loss: 10.8372
    Epoch 47/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.1558 - val_loss: 10.7150
    Epoch 48/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.1384 - val_loss: 9.8787
    Epoch 49/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.1687 - val_loss: 8.4732
    Epoch 50/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.1410 - val_loss: 10.1955
    Epoch 51/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.0743 - val_loss: 10.8531
    Epoch 52/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.0138 - val_loss: 9.8789
    Epoch 53/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.0038 - val_loss: 8.9808
    Epoch 54/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.0069 - val_loss: 9.7039
    Epoch 55/60
    4/4 [==============================] - 0s 19ms/step - loss: 4.9095 - val_loss: 9.9663
    Epoch 56/60
    4/4 [==============================] - 0s 18ms/step - loss: 4.9392 - val_loss: 10.5681
    Epoch 57/60
    4/4 [==============================] - 0s 17ms/step - loss: 4.8440 - val_loss: 9.1692
    Epoch 58/60
    4/4 [==============================] - 0s 18ms/step - loss: 4.8512 - val_loss: 9.1426
    Epoch 59/60
    4/4 [==============================] - 0s 18ms/step - loss: 4.9449 - val_loss: 10.2377
    Epoch 60/60
    4/4 [==============================] - 0s 16ms/step - loss: 4.8383 - val_loss: 7.8350
    Validation Loss for Interval 9:
    [2858.638671875, 2087.539306640625, 1367.8726806640625, 713.215576171875, 210.72422790527344, 20.255224227905273, 125.61463165283203, 197.41702270507812, 110.35214233398438, 27.443784713745117, 12.23721694946289, 22.513256072998047, 23.558320999145508, 16.540693283081055, 13.740297317504883, 16.835969924926758, 17.880277633666992, 16.248727798461914, 13.299689292907715, 12.122142791748047, 11.584864616394043, 11.049517631530762, 10.816278457641602, 12.14553451538086, 13.781872749328613, 13.130977630615234, 12.290619850158691, 11.21615982055664, 10.714576721191406, 11.988961219787598, 11.57341480255127, 11.138609886169434, 11.845311164855957, 11.88961410522461, 10.591840744018555, 10.731701850891113, 10.795084953308105, 11.8187255859375, 12.172944068908691, 11.565577507019043, 9.944807052612305, 9.517065048217773, 11.153069496154785, 11.427990913391113, 10.006085395812988, 10.837175369262695, 10.7149658203125, 9.878669738769531, 8.47321605682373, 10.195470809936523, 10.853095054626465, 9.878924369812012, 8.9807710647583, 9.703904151916504, 9.966324806213379, 10.568096160888672, 9.169177055358887, 9.142645835876465, 10.237674713134766, 7.834965229034424]
    ========================================
    Decoded Forecasts for Interval 9 (Forecast Date: 2014-01-01):
    PRCP: [5.07067   4.960751  4.8042088 4.7704077] (Average: 4.90)
    TAVG: [71.689926 71.286964 70.75601  70.524506] (Average: 71.06)
    TMAX: [81.30459  80.858246 80.2586   79.9616  ] (Average: 80.60)
    TMIN: [59.26104  58.712616 57.961525 57.74611 ] (Average: 58.42)
    ========================================
    Epoch 1/60
    4/4 [==============================] - 1s 83ms/step - loss: 2218.4221 - val_loss: 1435.0337
    Epoch 2/60
    4/4 [==============================] - 0s 18ms/step - loss: 1107.8599 - val_loss: 569.8987
    Epoch 3/60
    4/4 [==============================] - 0s 18ms/step - loss: 371.4483 - val_loss: 126.3331
    Epoch 4/60
    4/4 [==============================] - 0s 16ms/step - loss: 58.0307 - val_loss: 54.8228
    Epoch 5/60
    4/4 [==============================] - 0s 18ms/step - loss: 66.5403 - val_loss: 99.9500
    Epoch 6/60
    4/4 [==============================] - 0s 17ms/step - loss: 117.2792 - val_loss: 65.6862
    Epoch 7/60
    4/4 [==============================] - 0s 19ms/step - loss: 74.1428 - val_loss: 13.9059
    Epoch 8/60
    4/4 [==============================] - 0s 17ms/step - loss: 22.6158 - val_loss: 8.0028
    Epoch 9/60
    4/4 [==============================] - 0s 19ms/step - loss: 10.6136 - val_loss: 29.6891
    Epoch 10/60
    4/4 [==============================] - 0s 28ms/step - loss: 18.4593 - val_loss: 45.0978
    Epoch 11/60
    4/4 [==============================] - 0s 18ms/step - loss: 22.7340 - val_loss: 40.4059
    Epoch 12/60
    4/4 [==============================] - 0s 19ms/step - loss: 16.1104 - val_loss: 22.1548
    Epoch 13/60
    4/4 [==============================] - 0s 20ms/step - loss: 7.1096 - val_loss: 7.8078
    Epoch 14/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.8630 - val_loss: 3.4304
    Epoch 15/60
    4/4 [==============================] - 0s 18ms/step - loss: 8.4333 - val_loss: 2.5167
    Epoch 16/60
    4/4 [==============================] - 0s 19ms/step - loss: 8.0924 - val_loss: 4.1893
    Epoch 17/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.9929 - val_loss: 7.5917
    Epoch 18/60
    4/4 [==============================] - 0s 17ms/step - loss: 4.9710 - val_loss: 11.5110
    Epoch 19/60
    4/4 [==============================] - 0s 19ms/step - loss: 5.3899 - val_loss: 13.7785
    Epoch 20/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.7698 - val_loss: 13.1117
    Epoch 21/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.2002 - val_loss: 9.6212
    Epoch 22/60
    4/4 [==============================] - 0s 19ms/step - loss: 4.7993 - val_loss: 7.5498
    Epoch 23/60
    4/4 [==============================] - 0s 19ms/step - loss: 4.7418 - val_loss: 6.3445
    Epoch 24/60
    4/4 [==============================] - 0s 17ms/step - loss: 5.1132 - val_loss: 6.5909
    Epoch 25/60
    4/4 [==============================] - 0s 18ms/step - loss: 4.8034 - val_loss: 8.4126
    Epoch 26/60
    4/4 [==============================] - 0s 17ms/step - loss: 4.6557 - val_loss: 8.5839
    Epoch 27/60
    4/4 [==============================] - 0s 18ms/step - loss: 4.4659 - val_loss: 7.9352
    Epoch 28/60
    4/4 [==============================] - 0s 19ms/step - loss: 4.7967 - val_loss: 8.1580
    Epoch 29/60
    4/4 [==============================] - 0s 17ms/step - loss: 4.6867 - val_loss: 8.6008
    Epoch 30/60
    4/4 [==============================] - 0s 19ms/step - loss: 4.7146 - val_loss: 5.1109
    Epoch 31/60
    4/4 [==============================] - 0s 16ms/step - loss: 4.6757 - val_loss: 4.7445
    Epoch 32/60
    4/4 [==============================] - 0s 18ms/step - loss: 5.4584 - val_loss: 6.8915
    Epoch 33/60
    4/4 [==============================] - 0s 19ms/step - loss: 4.3809 - val_loss: 8.3129
    Epoch 34/60
    4/4 [==============================] - 0s 17ms/step - loss: 4.4638 - val_loss: 7.9345
    Epoch 35/60
    4/4 [==============================] - 0s 19ms/step - loss: 4.2024 - val_loss: 7.8013
    Epoch 36/60
    4/4 [==============================] - 0s 28ms/step - loss: 4.2891 - val_loss: 7.1737
    Epoch 37/60
    4/4 [==============================] - 0s 17ms/step - loss: 4.0828 - val_loss: 3.9195
    Epoch 38/60
    4/4 [==============================] - 0s 19ms/step - loss: 4.5520 - val_loss: 3.3717
    Epoch 39/60
    4/4 [==============================] - 0s 17ms/step - loss: 4.1704 - val_loss: 7.1642
    Epoch 40/60
    4/4 [==============================] - 0s 19ms/step - loss: 4.7367 - val_loss: 10.5605
    Epoch 41/60
    4/4 [==============================] - 0s 18ms/step - loss: 4.8844 - val_loss: 8.3990
    Epoch 42/60
    4/4 [==============================] - 0s 16ms/step - loss: 4.4070 - val_loss: 6.4543
    Epoch 43/60
    4/4 [==============================] - 0s 18ms/step - loss: 4.4888 - val_loss: 6.5041
    Epoch 44/60
    4/4 [==============================] - 0s 17ms/step - loss: 3.9765 - val_loss: 7.0268
    Epoch 45/60
    4/4 [==============================] - 0s 18ms/step - loss: 3.8981 - val_loss: 4.1116
    Epoch 46/60
    4/4 [==============================] - 0s 19ms/step - loss: 3.9675 - val_loss: 3.9010
    Epoch 47/60
    4/4 [==============================] - 0s 21ms/step - loss: 4.0655 - val_loss: 5.9690
    Epoch 48/60
    4/4 [==============================] - 0s 17ms/step - loss: 3.7601 - val_loss: 5.4525
    Epoch 49/60
    4/4 [==============================] - 0s 19ms/step - loss: 3.6096 - val_loss: 4.3870
    Epoch 50/60
    4/4 [==============================] - 0s 19ms/step - loss: 3.7563 - val_loss: 5.1362
    Epoch 51/60
    4/4 [==============================] - 0s 27ms/step - loss: 3.5056 - val_loss: 5.4154
    Epoch 52/60
    4/4 [==============================] - 0s 21ms/step - loss: 4.7007 - val_loss: 3.9856
    Epoch 53/60
    4/4 [==============================] - 0s 19ms/step - loss: 3.7877 - val_loss: 5.1723
    Epoch 54/60
    4/4 [==============================] - 0s 19ms/step - loss: 3.7595 - val_loss: 6.6409
    Epoch 55/60
    4/4 [==============================] - 0s 28ms/step - loss: 3.5421 - val_loss: 5.5718
    Epoch 56/60
    4/4 [==============================] - 0s 16ms/step - loss: 3.8970 - val_loss: 3.9611
    Epoch 57/60
    4/4 [==============================] - 0s 17ms/step - loss: 3.3868 - val_loss: 5.4166
    Epoch 58/60
    4/4 [==============================] - 0s 18ms/step - loss: 3.4641 - val_loss: 5.4689
    Epoch 59/60
    4/4 [==============================] - 0s 17ms/step - loss: 3.1891 - val_loss: 4.1667
    Epoch 60/60
    4/4 [==============================] - 0s 17ms/step - loss: 3.2632 - val_loss: 4.5859
    Validation Loss for Interval 10:
    [1435.03369140625, 569.8987426757812, 126.33308410644531, 54.822811126708984, 99.95001983642578, 65.68624114990234, 13.905925750732422, 8.00283432006836, 29.689105987548828, 45.097816467285156, 40.405941009521484, 22.154760360717773, 7.807772159576416, 3.430433988571167, 2.5166759490966797, 4.189289569854736, 7.591732025146484, 11.510997772216797, 13.778480529785156, 13.111689567565918, 9.621183395385742, 7.549833297729492, 6.344501495361328, 6.590938091278076, 8.412582397460938, 8.583877563476562, 7.935206890106201, 8.157951354980469, 8.6007661819458, 5.110916614532471, 4.744524002075195, 6.891479969024658, 8.312931060791016, 7.934483051300049, 7.801289081573486, 7.173703670501709, 3.919512987136841, 3.3717241287231445, 7.16420841217041, 10.560502052307129, 8.398992538452148, 6.454280376434326, 6.5040998458862305, 7.0268120765686035, 4.111628532409668, 3.9010062217712402, 5.968954086303711, 5.452508926391602, 4.386995315551758, 5.1361565589904785, 5.415426731109619, 3.985635757446289, 5.172327995300293, 6.640854358673096, 5.57182502746582, 3.9611153602600098, 5.416630744934082, 5.468908786773682, 4.166724681854248, 4.585883617401123]
    ========================================
    Decoded Forecasts for Interval 10 (Forecast Date: 2015-01-01):
    PRCP: [6.5938044 6.597267  6.6328464 6.554683 ] (Average: 6.59)
    TAVG: [72.444305 71.92274  70.97719  69.05479 ] (Average: 71.10)
    TMAX: [83.402405 82.73306  81.71748  79.51782 ] (Average: 81.84)
    TMIN: [59.02266  58.70342  58.635525 57.8486  ] (Average: 58.55)
    ========================================
    Epoch 1/60
    3/3 [==============================] - 1s 116ms/step - loss: 3416.4626 - val_loss: 3003.7336
    Epoch 2/60
    3/3 [==============================] - 0s 25ms/step - loss: 2751.3613 - val_loss: 2455.0681
    Epoch 3/60
    3/3 [==============================] - 0s 26ms/step - loss: 2242.7510 - val_loss: 1978.0197
    Epoch 4/60
    3/3 [==============================] - 0s 26ms/step - loss: 1802.7974 - val_loss: 1532.5900
    Epoch 5/60
    3/3 [==============================] - 0s 27ms/step - loss: 1370.5239 - val_loss: 1079.3550
    Epoch 6/60
    3/3 [==============================] - 0s 26ms/step - loss: 933.2866 - val_loss: 643.9885
    Epoch 7/60
    3/3 [==============================] - 0s 24ms/step - loss: 529.8691 - val_loss: 280.4190
    Epoch 8/60
    3/3 [==============================] - 0s 25ms/step - loss: 212.5279 - val_loss: 58.5638
    Epoch 9/60
    3/3 [==============================] - 0s 29ms/step - loss: 42.6247 - val_loss: 18.4786
    Epoch 10/60
    3/3 [==============================] - 0s 27ms/step - loss: 36.4929 - val_loss: 106.7540
    Epoch 11/60
    3/3 [==============================] - 0s 25ms/step - loss: 111.2217 - val_loss: 173.0897
    Epoch 12/60
    3/3 [==============================] - 0s 26ms/step - loss: 139.0097 - val_loss: 139.9731
    Epoch 13/60
    3/3 [==============================] - 0s 23ms/step - loss: 92.6542 - val_loss: 66.2472
    Epoch 14/60
    3/3 [==============================] - 0s 26ms/step - loss: 35.0741 - val_loss: 18.7561
    Epoch 15/60
    3/3 [==============================] - 0s 28ms/step - loss: 9.4572 - val_loss: 9.0168
    Epoch 16/60
    3/3 [==============================] - 0s 27ms/step - loss: 12.3649 - val_loss: 16.7099
    Epoch 17/60
    3/3 [==============================] - 0s 25ms/step - loss: 22.0608 - val_loss: 22.7464
    Epoch 18/60
    3/3 [==============================] - 0s 28ms/step - loss: 24.8666 - val_loss: 21.1333
    Epoch 19/60
    3/3 [==============================] - 0s 26ms/step - loss: 19.8192 - val_loss: 15.3182
    Epoch 20/60
    3/3 [==============================] - 0s 28ms/step - loss: 12.0721 - val_loss: 10.6912
    Epoch 21/60
    3/3 [==============================] - 0s 25ms/step - loss: 6.9738 - val_loss: 9.9713
    Epoch 22/60
    3/3 [==============================] - 0s 24ms/step - loss: 6.4854 - val_loss: 12.2177
    Epoch 23/60
    3/3 [==============================] - 0s 25ms/step - loss: 7.9592 - val_loss: 13.5383
    Epoch 24/60
    3/3 [==============================] - 0s 27ms/step - loss: 8.5237 - val_loss: 12.6918
    Epoch 25/60
    3/3 [==============================] - 0s 25ms/step - loss: 7.5505 - val_loss: 10.5480
    Epoch 26/60
    3/3 [==============================] - 0s 24ms/step - loss: 6.2239 - val_loss: 9.3786
    Epoch 27/60
    3/3 [==============================] - 0s 25ms/step - loss: 5.5704 - val_loss: 8.7623
    Epoch 28/60
    3/3 [==============================] - 0s 28ms/step - loss: 5.6531 - val_loss: 8.2215
    Epoch 29/60
    3/3 [==============================] - 0s 24ms/step - loss: 5.8931 - val_loss: 7.7951
    Epoch 30/60
    3/3 [==============================] - 0s 29ms/step - loss: 5.7778 - val_loss: 8.2393
    Epoch 31/60
    3/3 [==============================] - 0s 27ms/step - loss: 5.4772 - val_loss: 8.5245
    Epoch 32/60
    3/3 [==============================] - 0s 24ms/step - loss: 5.2810 - val_loss: 8.4505
    Epoch 33/60
    3/3 [==============================] - 0s 40ms/step - loss: 5.2651 - val_loss: 8.1058
    Epoch 34/60
    3/3 [==============================] - 0s 26ms/step - loss: 5.2784 - val_loss: 8.3570
    Epoch 35/60
    3/3 [==============================] - 0s 25ms/step - loss: 5.2313 - val_loss: 8.1353
    Epoch 36/60
    3/3 [==============================] - 0s 27ms/step - loss: 5.1803 - val_loss: 8.0703
    Epoch 37/60
    3/3 [==============================] - 0s 24ms/step - loss: 5.1416 - val_loss: 8.6155
    Epoch 38/60
    3/3 [==============================] - 0s 27ms/step - loss: 5.1130 - val_loss: 8.3569
    Epoch 39/60
    3/3 [==============================] - 0s 25ms/step - loss: 5.1319 - val_loss: 8.2748
    Epoch 40/60
    3/3 [==============================] - 0s 26ms/step - loss: 5.0669 - val_loss: 7.4142
    Epoch 41/60
    3/3 [==============================] - 0s 25ms/step - loss: 5.0197 - val_loss: 7.1756
    Epoch 42/60
    3/3 [==============================] - 0s 26ms/step - loss: 5.0305 - val_loss: 7.8723
    Epoch 43/60
    3/3 [==============================] - 0s 25ms/step - loss: 4.9860 - val_loss: 8.2807
    Epoch 44/60
    3/3 [==============================] - 0s 28ms/step - loss: 4.9676 - val_loss: 7.8980
    Epoch 45/60
    3/3 [==============================] - 0s 28ms/step - loss: 4.9372 - val_loss: 7.5517
    Epoch 46/60
    3/3 [==============================] - 0s 24ms/step - loss: 4.9139 - val_loss: 7.4652
    Epoch 47/60
    3/3 [==============================] - 0s 25ms/step - loss: 4.8771 - val_loss: 7.5980
    Epoch 48/60
    3/3 [==============================] - 0s 27ms/step - loss: 4.8864 - val_loss: 8.0769
    Epoch 49/60
    3/3 [==============================] - 0s 28ms/step - loss: 4.8488 - val_loss: 7.9305
    Epoch 50/60
    3/3 [==============================] - 0s 25ms/step - loss: 4.8411 - val_loss: 7.4386
    Epoch 51/60
    3/3 [==============================] - 0s 27ms/step - loss: 4.8017 - val_loss: 6.9751
    Epoch 52/60
    3/3 [==============================] - 0s 26ms/step - loss: 4.8099 - val_loss: 7.0583
    Epoch 53/60
    3/3 [==============================] - 0s 26ms/step - loss: 4.7424 - val_loss: 7.8482
    Epoch 54/60
    3/3 [==============================] - 0s 26ms/step - loss: 4.7358 - val_loss: 7.7301
    Epoch 55/60
    3/3 [==============================] - 0s 41ms/step - loss: 4.7116 - val_loss: 7.4789
    Epoch 56/60
    3/3 [==============================] - 0s 26ms/step - loss: 4.7086 - val_loss: 7.0168
    Epoch 57/60
    3/3 [==============================] - 0s 26ms/step - loss: 4.6705 - val_loss: 7.0529
    Epoch 58/60
    3/3 [==============================] - 0s 24ms/step - loss: 4.6400 - val_loss: 7.2191
    Epoch 59/60
    3/3 [==============================] - 0s 24ms/step - loss: 4.6174 - val_loss: 7.4600
    Epoch 60/60
    3/3 [==============================] - 0s 27ms/step - loss: 4.6045 - val_loss: 7.5035
    Validation Loss for Interval 11:
    [3003.733642578125, 2455.068115234375, 1978.0196533203125, 1532.5899658203125, 1079.35498046875, 643.9884643554688, 280.4189758300781, 58.563751220703125, 18.47864532470703, 106.75395202636719, 173.08970642089844, 139.97305297851562, 66.24723815917969, 18.756101608276367, 9.016826629638672, 16.709901809692383, 22.74639129638672, 21.133296966552734, 15.318212509155273, 10.691205978393555, 9.971341133117676, 12.217728614807129, 13.538331031799316, 12.691781997680664, 10.547998428344727, 9.378600120544434, 8.762286186218262, 8.221458435058594, 7.7950968742370605, 8.239317893981934, 8.524505615234375, 8.45053482055664, 8.105813980102539, 8.357043266296387, 8.135261535644531, 8.070296287536621, 8.615485191345215, 8.356880187988281, 8.274801254272461, 7.4142165184021, 7.175609588623047, 7.8722758293151855, 8.280704498291016, 7.8979716300964355, 7.551731109619141, 7.465193271636963, 7.5979695320129395, 8.076924324035645, 7.9304518699646, 7.438580513000488, 6.975137233734131, 7.058261871337891, 7.848156452178955, 7.730052947998047, 7.4788899421691895, 7.016777515411377, 7.052920341491699, 7.219140529632568, 7.460009574890137, 7.503528118133545]
    ========================================
    Decoded Forecasts for Interval 11 (Forecast Date: 2016-01-01):
    PRCP: [5.2988906] (Average: 5.30)
    TAVG: [69.11568] (Average: 69.12)
    TMAX: [79.343864] (Average: 79.34)
    TMIN: [57.772556] (Average: 57.77)
    ========================================
    Epoch 1/60
    3/3 [==============================] - 1s 116ms/step - loss: 3063.9778 - val_loss: 2599.7834
    Epoch 2/60
    3/3 [==============================] - 0s 27ms/step - loss: 2322.4250 - val_loss: 1936.6929
    Epoch 3/60
    3/3 [==============================] - 0s 26ms/step - loss: 1697.5419 - val_loss: 1326.1450
    Epoch 4/60
    3/3 [==============================] - 0s 24ms/step - loss: 1120.9924 - val_loss: 787.1566
    Epoch 5/60
    3/3 [==============================] - 0s 26ms/step - loss: 633.0577 - val_loss: 364.4011
    Epoch 6/60
    3/3 [==============================] - 0s 25ms/step - loss: 267.7345 - val_loss: 104.8835
    Epoch 7/60
    3/3 [==============================] - 0s 26ms/step - loss: 69.7206 - val_loss: 26.5063
    Epoch 8/60
    3/3 [==============================] - 0s 23ms/step - loss: 35.3930 - val_loss: 72.0290
    Epoch 9/60
    3/3 [==============================] - 0s 24ms/step - loss: 85.4670 - val_loss: 125.1807
    Epoch 10/60
    3/3 [==============================] - 0s 27ms/step - loss: 117.0176 - val_loss: 118.6110
    Epoch 11/60
    3/3 [==============================] - 0s 24ms/step - loss: 95.7126 - val_loss: 73.3691
    Epoch 12/60
    3/3 [==============================] - 0s 27ms/step - loss: 52.6896 - val_loss: 35.5649
    Epoch 13/60
    3/3 [==============================] - 0s 24ms/step - loss: 23.9812 - val_loss: 19.7528
    Epoch 14/60
    3/3 [==============================] - 0s 27ms/step - loss: 15.5761 - val_loss: 19.3280
    Epoch 15/60
    3/3 [==============================] - 0s 25ms/step - loss: 17.4121 - val_loss: 21.4542
    Epoch 16/60
    3/3 [==============================] - 0s 28ms/step - loss: 19.8074 - val_loss: 21.6931
    Epoch 17/60
    3/3 [==============================] - 0s 25ms/step - loss: 18.7105 - val_loss: 19.3746
    Epoch 18/60
    3/3 [==============================] - 0s 28ms/step - loss: 15.5477 - val_loss: 15.6421
    Epoch 19/60
    3/3 [==============================] - 0s 25ms/step - loss: 12.2305 - val_loss: 13.1569
    Epoch 20/60
    3/3 [==============================] - 0s 27ms/step - loss: 9.4975 - val_loss: 11.6538
    Epoch 21/60
    3/3 [==============================] - 0s 25ms/step - loss: 8.3631 - val_loss: 11.1799
    Epoch 22/60
    3/3 [==============================] - 0s 25ms/step - loss: 8.0522 - val_loss: 10.7603
    Epoch 23/60
    3/3 [==============================] - 0s 25ms/step - loss: 8.4181 - val_loss: 11.1309
    Epoch 24/60
    3/3 [==============================] - 0s 25ms/step - loss: 8.3905 - val_loss: 11.1914
    Epoch 25/60
    3/3 [==============================] - 0s 24ms/step - loss: 7.8969 - val_loss: 10.5319
    Epoch 26/60
    3/3 [==============================] - 0s 28ms/step - loss: 7.2893 - val_loss: 9.9883
    Epoch 27/60
    3/3 [==============================] - 0s 26ms/step - loss: 6.9770 - val_loss: 9.9021
    Epoch 28/60
    3/3 [==============================] - 0s 26ms/step - loss: 7.0720 - val_loss: 9.8122
    Epoch 29/60
    3/3 [==============================] - 0s 24ms/step - loss: 7.0585 - val_loss: 9.9897
    Epoch 30/60
    3/3 [==============================] - 0s 27ms/step - loss: 6.9598 - val_loss: 9.7236
    Epoch 31/60
    3/3 [==============================] - 0s 24ms/step - loss: 6.8308 - val_loss: 9.2018
    Epoch 32/60
    3/3 [==============================] - 0s 25ms/step - loss: 6.6491 - val_loss: 9.0796
    Epoch 33/60
    3/3 [==============================] - 0s 25ms/step - loss: 6.5485 - val_loss: 8.8957
    Epoch 34/60
    3/3 [==============================] - 0s 23ms/step - loss: 6.4802 - val_loss: 9.3945
    Epoch 35/60
    3/3 [==============================] - 0s 25ms/step - loss: 6.4849 - val_loss: 10.1211
    Epoch 36/60
    3/3 [==============================] - 0s 26ms/step - loss: 6.4784 - val_loss: 9.6600
    Epoch 37/60
    3/3 [==============================] - 0s 35ms/step - loss: 6.3304 - val_loss: 8.6546
    Epoch 38/60
    3/3 [==============================] - 0s 24ms/step - loss: 6.1605 - val_loss: 8.1217
    Epoch 39/60
    3/3 [==============================] - 0s 24ms/step - loss: 6.1324 - val_loss: 7.9659
    Epoch 40/60
    3/3 [==============================] - 0s 35ms/step - loss: 6.1225 - val_loss: 7.9522
    Epoch 41/60
    3/3 [==============================] - 0s 26ms/step - loss: 6.0259 - val_loss: 8.7064
    Epoch 42/60
    3/3 [==============================] - 0s 26ms/step - loss: 6.0113 - val_loss: 9.0170
    Epoch 43/60
    3/3 [==============================] - 0s 26ms/step - loss: 5.9908 - val_loss: 8.3845
    Epoch 44/60
    3/3 [==============================] - 0s 23ms/step - loss: 6.0488 - val_loss: 7.3140
    Epoch 45/60
    3/3 [==============================] - 0s 25ms/step - loss: 5.9529 - val_loss: 7.7048
    Epoch 46/60
    3/3 [==============================] - 0s 28ms/step - loss: 5.8898 - val_loss: 9.1094
    Epoch 47/60
    3/3 [==============================] - 0s 26ms/step - loss: 5.8898 - val_loss: 8.7790
    Epoch 48/60
    3/3 [==============================] - 0s 27ms/step - loss: 5.8240 - val_loss: 7.8400
    Epoch 49/60
    3/3 [==============================] - 0s 24ms/step - loss: 5.7595 - val_loss: 7.0762
    Epoch 50/60
    3/3 [==============================] - 0s 26ms/step - loss: 5.7399 - val_loss: 7.1243
    Epoch 51/60
    3/3 [==============================] - 0s 26ms/step - loss: 5.7251 - val_loss: 8.0950
    Epoch 52/60
    3/3 [==============================] - 0s 27ms/step - loss: 5.6533 - val_loss: 7.8862
    Epoch 53/60
    3/3 [==============================] - 0s 24ms/step - loss: 5.5780 - val_loss: 7.0575
    Epoch 54/60
    3/3 [==============================] - 0s 25ms/step - loss: 5.4626 - val_loss: 7.0187
    Epoch 55/60
    3/3 [==============================] - 0s 26ms/step - loss: 5.4405 - val_loss: 7.5046
    Epoch 56/60
    3/3 [==============================] - 0s 25ms/step - loss: 5.4186 - val_loss: 7.6054
    Epoch 57/60
    3/3 [==============================] - 0s 27ms/step - loss: 5.3608 - val_loss: 6.8083
    Epoch 58/60
    3/3 [==============================] - 0s 28ms/step - loss: 5.3429 - val_loss: 6.2198
    Epoch 59/60
    3/3 [==============================] - 0s 23ms/step - loss: 5.3649 - val_loss: 6.4088
    Epoch 60/60
    3/3 [==============================] - 0s 25ms/step - loss: 5.2618 - val_loss: 7.6247
    Validation Loss for Interval 12:
    [2599.783447265625, 1936.69287109375, 1326.14501953125, 787.1566162109375, 364.40106201171875, 104.8835220336914, 26.50629234313965, 72.0289535522461, 125.18073272705078, 118.61103820800781, 73.36913299560547, 35.56487274169922, 19.752836227416992, 19.32798957824707, 21.454235076904297, 21.69305992126465, 19.37458610534668, 15.642060279846191, 13.156937599182129, 11.653809547424316, 11.179932594299316, 10.760321617126465, 11.130908012390137, 11.191433906555176, 10.531917572021484, 9.988262176513672, 9.902115821838379, 9.81216812133789, 9.989668846130371, 9.723570823669434, 9.20180606842041, 9.079649925231934, 8.895689010620117, 9.394527435302734, 10.121091842651367, 9.659981727600098, 8.654559135437012, 8.121655464172363, 7.965919017791748, 7.9522175788879395, 8.706412315368652, 9.017045021057129, 8.384536743164062, 7.313988208770752, 7.704847812652588, 9.109359741210938, 8.779040336608887, 7.839988708496094, 7.076233386993408, 7.124311923980713, 8.095026969909668, 7.886229038238525, 7.057482719421387, 7.018716812133789, 7.504646301269531, 7.605406284332275, 6.808315753936768, 6.21981954574585, 6.408825874328613, 7.624678134918213]
    ========================================
    Decoded Forecasts for Interval 12 (Forecast Date: 2017-01-01):
    PRCP: [5.418084  5.3969254 5.416485 ] (Average: 5.41)
    TAVG: [69.367386 70.43264  68.99492 ] (Average: 69.60)
    TMAX: [78.923225 80.109535 78.51763 ] (Average: 79.18)
    TMIN: [57.21188  58.283436 56.8588  ] (Average: 57.45)
    ========================================
    Epoch 1/60
    3/3 [==============================] - 1s 118ms/step - loss: 3365.0027 - val_loss: 3004.3323
    Epoch 2/60
    3/3 [==============================] - 0s 29ms/step - loss: 2729.6492 - val_loss: 2390.6147
    Epoch 3/60
    3/3 [==============================] - 0s 26ms/step - loss: 2153.3801 - val_loss: 1811.5563
    Epoch 4/60
    3/3 [==============================] - 0s 26ms/step - loss: 1597.4807 - val_loss: 1236.4291
    Epoch 5/60
    3/3 [==============================] - 0s 41ms/step - loss: 1051.5938 - val_loss: 702.9310
    Epoch 6/60
    3/3 [==============================] - 0s 26ms/step - loss: 562.2920 - val_loss: 285.5816
    Epoch 7/60
    3/3 [==============================] - 0s 26ms/step - loss: 206.2075 - val_loss: 72.8081
    Epoch 8/60
    3/3 [==============================] - 0s 27ms/step - loss: 55.4566 - val_loss: 76.1657
    Epoch 9/60
    3/3 [==============================] - 0s 28ms/step - loss: 90.3697 - val_loss: 150.6853
    Epoch 10/60
    3/3 [==============================] - 0s 24ms/step - loss: 150.2852 - val_loss: 145.5959
    Epoch 11/60
    3/3 [==============================] - 0s 25ms/step - loss: 127.8744 - val_loss: 79.3975
    Epoch 12/60
    3/3 [==============================] - 0s 25ms/step - loss: 64.7106 - val_loss: 29.4082
    Epoch 13/60
    3/3 [==============================] - 0s 26ms/step - loss: 25.3904 - val_loss: 21.0419
    Epoch 14/60
    3/3 [==============================] - 0s 25ms/step - loss: 20.6191 - val_loss: 33.2777
    Epoch 15/60
    3/3 [==============================] - 0s 25ms/step - loss: 29.2663 - val_loss: 41.2457
    Epoch 16/60
    3/3 [==============================] - 0s 25ms/step - loss: 32.2093 - val_loss: 36.4687
    Epoch 17/60
    3/3 [==============================] - 0s 24ms/step - loss: 25.7724 - val_loss: 23.6232
    Epoch 18/60
    3/3 [==============================] - 0s 27ms/step - loss: 15.3258 - val_loss: 11.7605
    Epoch 19/60
    3/3 [==============================] - 0s 26ms/step - loss: 8.4643 - val_loss: 7.1332
    Epoch 20/60
    3/3 [==============================] - 0s 27ms/step - loss: 8.5131 - val_loss: 7.9396
    Epoch 21/60
    3/3 [==============================] - 0s 24ms/step - loss: 11.0125 - val_loss: 9.0825
    Epoch 22/60
    3/3 [==============================] - 0s 25ms/step - loss: 11.5741 - val_loss: 8.3707
    Epoch 23/60
    3/3 [==============================] - 0s 24ms/step - loss: 9.6750 - val_loss: 7.0801
    Epoch 24/60
    3/3 [==============================] - 0s 24ms/step - loss: 7.6392 - val_loss: 7.2610
    Epoch 25/60
    3/3 [==============================] - 0s 26ms/step - loss: 6.7846 - val_loss: 8.1951
    Epoch 26/60
    3/3 [==============================] - 0s 24ms/step - loss: 7.2309 - val_loss: 8.9783
    Epoch 27/60
    3/3 [==============================] - 0s 23ms/step - loss: 7.5034 - val_loss: 8.6102
    Epoch 28/60
    3/3 [==============================] - 0s 27ms/step - loss: 7.4042 - val_loss: 7.7450
    Epoch 29/60
    3/3 [==============================] - 0s 25ms/step - loss: 7.0514 - val_loss: 7.0358
    Epoch 30/60
    3/3 [==============================] - 0s 28ms/step - loss: 6.8043 - val_loss: 7.4705
    Epoch 31/60
    3/3 [==============================] - 0s 24ms/step - loss: 6.7358 - val_loss: 7.5629
    Epoch 32/60
    3/3 [==============================] - 0s 27ms/step - loss: 6.7455 - val_loss: 7.8745
    Epoch 33/60
    3/3 [==============================] - 0s 25ms/step - loss: 6.7666 - val_loss: 7.4506
    Epoch 34/60
    3/3 [==============================] - 0s 27ms/step - loss: 6.7082 - val_loss: 6.1587
    Epoch 35/60
    3/3 [==============================] - 0s 24ms/step - loss: 6.5589 - val_loss: 6.1848
    Epoch 36/60
    3/3 [==============================] - 0s 27ms/step - loss: 6.5466 - val_loss: 6.8311
    Epoch 37/60
    3/3 [==============================] - 0s 24ms/step - loss: 6.5147 - val_loss: 7.1696
    Epoch 38/60
    3/3 [==============================] - 0s 27ms/step - loss: 6.5024 - val_loss: 6.8514
    Epoch 39/60
    3/3 [==============================] - 0s 24ms/step - loss: 6.4321 - val_loss: 6.8002
    Epoch 40/60
    3/3 [==============================] - 0s 28ms/step - loss: 6.4075 - val_loss: 6.7257
    Epoch 41/60
    3/3 [==============================] - 0s 25ms/step - loss: 6.3677 - val_loss: 6.4895
    Epoch 42/60
    3/3 [==============================] - 0s 26ms/step - loss: 6.3901 - val_loss: 6.3832
    Epoch 43/60
    3/3 [==============================] - 0s 24ms/step - loss: 6.3570 - val_loss: 6.4776
    Epoch 44/60
    3/3 [==============================] - 0s 25ms/step - loss: 6.3278 - val_loss: 6.5521
    Epoch 45/60
    3/3 [==============================] - 0s 28ms/step - loss: 6.2675 - val_loss: 6.6799
    Epoch 46/60
    3/3 [==============================] - 0s 27ms/step - loss: 6.2188 - val_loss: 6.6515
    Epoch 47/60
    3/3 [==============================] - 0s 25ms/step - loss: 6.2322 - val_loss: 6.8482
    Epoch 48/60
    3/3 [==============================] - 0s 37ms/step - loss: 6.2315 - val_loss: 6.6790
    Epoch 49/60
    3/3 [==============================] - 0s 26ms/step - loss: 6.1800 - val_loss: 6.2338
    Epoch 50/60
    3/3 [==============================] - 0s 25ms/step - loss: 6.2503 - val_loss: 5.3501
    Epoch 51/60
    3/3 [==============================] - 0s 26ms/step - loss: 6.2298 - val_loss: 5.8746
    Epoch 52/60
    3/3 [==============================] - 0s 25ms/step - loss: 6.1510 - val_loss: 6.5353
    Epoch 53/60
    3/3 [==============================] - 0s 24ms/step - loss: 6.0775 - val_loss: 6.3930
    Epoch 54/60
    3/3 [==============================] - 0s 26ms/step - loss: 6.0783 - val_loss: 6.1452
    Epoch 55/60
    3/3 [==============================] - 0s 25ms/step - loss: 6.0171 - val_loss: 5.5182
    Epoch 56/60
    3/3 [==============================] - 0s 26ms/step - loss: 6.0337 - val_loss: 5.3578
    Epoch 57/60
    3/3 [==============================] - 0s 23ms/step - loss: 6.0118 - val_loss: 5.3930
    Epoch 58/60
    3/3 [==============================] - 0s 25ms/step - loss: 6.0075 - val_loss: 5.6156
    Epoch 59/60
    3/3 [==============================] - 0s 27ms/step - loss: 5.9564 - val_loss: 5.9703
    Epoch 60/60
    3/3 [==============================] - 0s 25ms/step - loss: 5.9041 - val_loss: 6.5350
    Validation Loss for Interval 13:
    [3004.332275390625, 2390.61474609375, 1811.5562744140625, 1236.4290771484375, 702.9310302734375, 285.58160400390625, 72.80806732177734, 76.1656723022461, 150.6852569580078, 145.59585571289062, 79.39754486083984, 29.408248901367188, 21.041934967041016, 33.2777214050293, 41.245670318603516, 36.468711853027344, 23.623220443725586, 11.760510444641113, 7.13322114944458, 7.939642429351807, 9.082493782043457, 8.370686531066895, 7.080135345458984, 7.261015892028809, 8.19510269165039, 8.978277206420898, 8.610208511352539, 7.744998931884766, 7.035755157470703, 7.470515251159668, 7.562921047210693, 7.874485015869141, 7.450567245483398, 6.158740997314453, 6.184751987457275, 6.83108377456665, 7.1695685386657715, 6.8514084815979, 6.800191879272461, 6.725699424743652, 6.489473342895508, 6.383243083953857, 6.477608680725098, 6.5521240234375, 6.679903030395508, 6.651488780975342, 6.848226547241211, 6.679027557373047, 6.233802318572998, 5.350063323974609, 5.874582767486572, 6.535292148590088, 6.392950534820557, 6.145208358764648, 5.5182366371154785, 5.357838153839111, 5.392962455749512, 5.615575790405273, 5.970280647277832, 6.535038471221924]
    ========================================
    Decoded Forecasts for Interval 13 (Forecast Date: 2018-01-01):
    PRCP: [6.104527  6.0388284 5.936825  6.2403383] (Average: 6.08)
    TAVG: [69.88872 70.19077 70.01759 68.68351] (Average: 69.70)
    TMAX: [80.18134  80.60227  80.27522  78.394325] (Average: 79.86)
    TMIN: [58.46757  58.74219  58.439457 57.221066] (Average: 58.22)
    ========================================
    


```python
data.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>DATE</th>
      <th>PRCP</th>
      <th>TAVG</th>
      <th>TMAX</th>
      <th>TMIN</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>319</th>
      <td>1985-01-01</td>
      <td>0.48</td>
      <td>67.3</td>
      <td>79.8</td>
      <td>54.7</td>
    </tr>
    <tr>
      <th>320</th>
      <td>1985-02-01</td>
      <td>5.56</td>
      <td>68.1</td>
      <td>79.3</td>
      <td>56.9</td>
    </tr>
    <tr>
      <th>321</th>
      <td>1985-03-01</td>
      <td>2.33</td>
      <td>68.1</td>
      <td>80.6</td>
      <td>56.9</td>
    </tr>
    <tr>
      <th>322</th>
      <td>1985-04-01</td>
      <td>7.46</td>
      <td>67.7</td>
      <td>76.7</td>
      <td>58.8</td>
    </tr>
    <tr>
      <th>323</th>
      <td>1985-05-01</td>
      <td>2.14</td>
      <td>67.7</td>
      <td>76.7</td>
      <td>58.8</td>
    </tr>
  </tbody>
</table>
</div>




```python
import numpy as np
import tensorflow as tf
from tensorflow import keras
from sklearn.model_selection import train_test_split
import pandas as pd

# Assuming you have your 'data' prepared and loaded with the appropriate shape

# Convert 'DATE' column to timestamp format
data['DATE'] = pd.to_datetime(data['DATE'])

# Set random seeds for reproducibility
tf.random.set_seed(42)
np.random.seed(42)

# Specify parameters
history_years = 20  # Number of years for historical data
forecast_year = 1   # Number of years to forecast
num_intervals = 13  # Number of intervals to repeat the process
interval_length = 365  # Length of each interval in days

# Batch size
batch_size = 32  # Adjust according to your computational resources and model characteristics

# Calculate the total length of data
total_years = history_years + forecast_year

# Create an empty list to store forecasting results
forecast_results = []

# Create an empty dictionary to store parameter predictions
parameter_predictions = {
    "PRCP": [],
    "TAVG": [],
    "TMAX": [],
    "TMIN": []
}

# Define the initial start date for the intervals
initial_start_date = pd.Timestamp("1985-01-01")

# Loop over different intervals
for interval in range(num_intervals):
    # Calculate the start and end dates for the historical period
    start_date = initial_start_date + pd.DateOffset(years=interval)
    end_date = start_date + pd.DateOffset(years=history_years)
    
    # Extract data for the current historical interval
    historical_data = data[(data['DATE'] >= start_date) & (data['DATE'] < end_date)]
    
    # Calculate the start and end dates for the forecast period
    forecast_start_date = end_date + pd.DateOffset(years=1)  # Add one year for uniform forecasting
    forecast_end_date = forecast_start_date + pd.DateOffset(years=1)
    
    # Extract data for the current forecast interval
    forecast_data = data[(data['DATE'] >= forecast_start_date) & (data['DATE'] < forecast_end_date)]
    
    # Split historical data into train and test sets
    train_data, test_data = train_test_split(historical_data, test_size=0.2, shuffle=False)
    
    # Create Stacked Denoising Autoencoder
    your_input_shape = historical_data.shape[1] - 1  
    your_output_shape = your_input_shape  # Define your output shape here
    
    denoising_encoder = keras.models.Sequential([
        keras.layers.Flatten(input_shape=[your_input_shape]),
        keras.layers.GaussianNoise(0.2),
        keras.layers.Dense(100, activation="selu"),
        keras.layers.Dense(30, activation="selu")
    ])
    
    denoising_decoder = keras.models.Sequential([
        keras.layers.Dense(100, activation="selu", input_shape=[30]),
        keras.layers.Dense(your_output_shape, activation="linear"),  # Use linear activation for output layer
        keras.layers.Reshape([your_output_shape])
    ])
    
    denoising_ae = keras.models.Sequential([denoising_encoder, denoising_decoder])
    denoising_ae.compile(loss="mean_squared_error", optimizer=keras.optimizers.Adam(learning_rate=0.001))
    
    # Train the autoencoder on train data with validation loss monitoring
    history = denoising_ae.fit(train_data.drop('DATE', axis=1), train_data.drop('DATE', axis=1),
                                epochs=60, batch_size=32,
                                validation_data=(test_data.drop('DATE', axis=1), test_data.drop('DATE', axis=1)),
                                verbose=1)  # Set verbose to 1 to see training progress
    
    # Display validation loss for each epoch
    print(f"Validation Loss for Interval {interval + 1}:")
    print(history.history['val_loss'])
    print("=" * 40)

    # Use the trained autoencoder for forecasting
    encoded_forecast = denoising_ae.layers[0](forecast_data.drop('DATE', axis=1).values)  # Access encoder layers
    decoded_forecast = denoising_ae.layers[1](encoded_forecast)  # Access decoder layers
    
    # Store the decoded forecast results for this interval
    forecast_results.append(decoded_forecast)

    # Display parameter predictions for this interval
    print(f"Decoded Forecasts for Interval {interval + 1} (Forecast Date: {forecast_start_date.date()}):")
    for param_idx, param_name in enumerate(["PRCP", "TAVG", "TMAX", "TMIN"]):
        param_prediction = decoded_forecast[:, param_idx]
        parameter_predictions[param_name].extend(param_prediction)
        avg_param_prediction = np.mean(param_prediction)  # Calculate average prediction
        print(f"{param_name}: {param_prediction} (Average: {avg_param_prediction:.2f})")
    print("=" * 40)

    # Move the initial start date for the next interval
    initial_start_date += pd.DateOffset(years=0)

```

    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m2s[0m 69ms/step - loss: 3582.1914 - val_loss: 2924.4016
    Epoch 2/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2590.9165 - val_loss: 2095.8066
    Epoch 3/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1812.5050 - val_loss: 1290.5875
    Epoch 4/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1050.2144 - val_loss: 531.5864
    Epoch 5/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 14ms/step - loss: 379.4989 - val_loss: 70.5844
    Epoch 6/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 37.9345 - val_loss: 58.4581
    Epoch 7/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 81.9177 - val_loss: 131.5163
    Epoch 8/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 7ms/step - loss: 114.7264 - val_loss: 45.4391
    Epoch 9/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 31.5713 - val_loss: 8.9178
    Epoch 10/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 6ms/step - loss: 8.9605 - val_loss: 26.8806
    Epoch 11/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 22.5653 - val_loss: 26.6701
    Epoch 12/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 18.7099 - val_loss: 11.8761
    Epoch 13/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 7.8778 - val_loss: 7.4909
    Epoch 14/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 7ms/step - loss: 6.7571 - val_loss: 10.1536
    Epoch 15/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 8.5070 - val_loss: 8.8804
    Epoch 16/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.6869 - val_loss: 7.4995
    Epoch 17/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 6ms/step - loss: 5.6819 - val_loss: 8.2148
    Epoch 18/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 6.0593 - val_loss: 8.3294
    Epoch 19/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 5.8450 - val_loss: 7.6425
    Epoch 20/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 5.4924 - val_loss: 7.3524
    Epoch 21/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 5.5047 - val_loss: 7.2875
    Epoch 22/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 5.3810 - val_loss: 7.1152
    Epoch 23/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 5.1399 - val_loss: 7.1940
    Epoch 24/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 6ms/step - loss: 5.1042 - val_loss: 7.1598
    Epoch 25/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 5.0682 - val_loss: 6.9841
    Epoch 26/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 4.9732 - val_loss: 7.0592
    Epoch 27/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 4.9549 - val_loss: 6.8448
    Epoch 28/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 4.8595 - val_loss: 6.7886
    Epoch 29/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 4.7873 - val_loss: 6.8376
    Epoch 30/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.7515 - val_loss: 6.7723
    Epoch 31/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 15ms/step - loss: 4.6883 - val_loss: 6.5503
    Epoch 32/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.6069 - val_loss: 6.5476
    Epoch 33/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.5695 - val_loss: 6.5550
    Epoch 34/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 4.4896 - val_loss: 6.4384
    Epoch 35/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 4.3675 - val_loss: 6.2775
    Epoch 36/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.2959 - val_loss: 6.2494
    Epoch 37/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 4.2235 - val_loss: 6.2229
    Epoch 38/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 4.1650 - val_loss: 6.2257
    Epoch 39/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 4.1103 - val_loss: 6.1046
    Epoch 40/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 4.0512 - val_loss: 6.0128
    Epoch 41/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 3.9756 - val_loss: 5.9864
    Epoch 42/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.9216 - val_loss: 5.9269
    Epoch 43/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.8570 - val_loss: 5.8843
    Epoch 44/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.7954 - val_loss: 5.7954
    Epoch 45/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 3.7442 - val_loss: 5.7882
    Epoch 46/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.6869 - val_loss: 5.7028
    Epoch 47/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 3.6235 - val_loss: 5.6923
    Epoch 48/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.5836 - val_loss: 5.5692
    Epoch 49/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.5033 - val_loss: 5.5182
    Epoch 50/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 3.4439 - val_loss: 5.4493
    Epoch 51/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.4069 - val_loss: 5.4186
    Epoch 52/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 3.3293 - val_loss: 5.2953
    Epoch 53/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.2599 - val_loss: 5.2000
    Epoch 54/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.2046 - val_loss: 5.1147
    Epoch 55/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 3.1384 - val_loss: 5.1107
    Epoch 56/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.1008 - val_loss: 4.9902
    Epoch 57/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 3.0343 - val_loss: 4.9065
    Epoch 58/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2.9472 - val_loss: 4.8967
    Epoch 59/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 2.8459 - val_loss: 4.7430
    Epoch 60/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 2.7151 - val_loss: 4.6902
    Validation Loss for Interval 1:
    [2924.401611328125, 2095.806640625, 1290.5875244140625, 531.58642578125, 70.5844497680664, 58.4581184387207, 131.51629638671875, 45.43911361694336, 8.917798042297363, 26.880605697631836, 26.670108795166016, 11.876138687133789, 7.4908766746521, 10.153571128845215, 8.880363464355469, 7.499460220336914, 8.214803695678711, 8.329368591308594, 7.642458438873291, 7.352407455444336, 7.287517547607422, 7.115178108215332, 7.194006443023682, 7.159814357757568, 6.9840545654296875, 7.0591721534729, 6.844789028167725, 6.788631439208984, 6.837599754333496, 6.772337436676025, 6.550311088562012, 6.5475945472717285, 6.555039405822754, 6.438435077667236, 6.2775492668151855, 6.249448776245117, 6.222906112670898, 6.225718975067139, 6.104637622833252, 6.012812614440918, 5.986417293548584, 5.92689847946167, 5.884296417236328, 5.795440673828125, 5.788180828094482, 5.702810287475586, 5.692299842834473, 5.569177150726318, 5.518187522888184, 5.449321269989014, 5.418636798858643, 5.295334339141846, 5.200033664703369, 5.114721775054932, 5.110703468322754, 4.990202903747559, 4.906501293182373, 4.896749496459961, 4.7429585456848145, 4.690176486968994]
    ========================================
    Decoded Forecasts for Interval 1 (Forecast Date: 2006-01-01):
    PRCP: [3.7600052 3.7504823 3.24679   3.3569705 3.0222435 3.702176  5.1283183
     5.106265 ] (Average: 3.88)
    TAVG: [68.537926 68.53666  68.6117   67.16807  67.09629  68.882286 68.8
     68.963615] (Average: 68.32)
    TMAX: [81.49289  81.41849  77.24654  76.95772  74.36391  81.343765 81.312325
     81.25548 ] (Average: 79.42)
    TMIN: [56.297554 56.300606 56.93508  55.531204 55.647892 56.63607  56.51386
     56.69796 ] (Average: 56.32)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m2s[0m 59ms/step - loss: 2447.0537 - val_loss: 1805.4130
    Epoch 2/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1532.5026 - val_loss: 873.4867
    Epoch 3/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 679.9772 - val_loss: 214.5215
    Epoch 4/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 155.7829 - val_loss: 74.5434
    Epoch 5/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 81.9442 - val_loss: 102.6665
    Epoch 6/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 84.6814 - val_loss: 55.3856
    Epoch 7/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 42.1267 - val_loss: 41.2543
    Epoch 8/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 33.5377 - val_loss: 27.0007
    Epoch 9/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 19.6754 - val_loss: 9.1128
    Epoch 10/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 9.3024 - val_loss: 12.8452
    Epoch 11/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 12.8436 - val_loss: 11.7345
    Epoch 12/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 8.6664 - val_loss: 7.5056
    Epoch 13/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 5.1764 - val_loss: 7.8741
    Epoch 14/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 5.9136 - val_loss: 7.0101
    Epoch 15/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 5.3845 - val_loss: 6.3330
    Epoch 16/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 4.9190 - val_loss: 6.4934
    Epoch 17/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 4.6961 - val_loss: 6.3510
    Epoch 18/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 4.4899 - val_loss: 6.0010
    Epoch 19/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 4.4227 - val_loss: 5.6003
    Epoch 20/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.2519 - val_loss: 5.4574
    Epoch 21/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 4.0945 - val_loss: 5.2869
    Epoch 22/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.9350 - val_loss: 5.1777
    Epoch 23/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 3.7971 - val_loss: 4.9031
    Epoch 24/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.6749 - val_loss: 4.6968
    Epoch 25/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.5768 - val_loss: 4.6064
    Epoch 26/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 3.4752 - val_loss: 4.4718
    Epoch 27/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 3.4035 - val_loss: 4.3184
    Epoch 28/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.3024 - val_loss: 4.1215
    Epoch 29/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.2055 - val_loss: 4.0059
    Epoch 30/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.1273 - val_loss: 3.8315
    Epoch 31/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.0368 - val_loss: 3.7822
    Epoch 32/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 2.9421 - val_loss: 3.6944
    Epoch 33/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2.8802 - val_loss: 3.6270
    Epoch 34/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2.7817 - val_loss: 3.4555
    Epoch 35/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 2.7339 - val_loss: 3.4372
    Epoch 36/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2.6440 - val_loss: 3.4196
    Epoch 37/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2.5927 - val_loss: 3.3457
    Epoch 38/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 2.5877 - val_loss: 3.2799
    Epoch 39/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 2.5315 - val_loss: 3.2460
    Epoch 40/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 2.4578 - val_loss: 3.2136
    Epoch 41/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2.3982 - val_loss: 3.0725
    Epoch 42/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 2.2229 - val_loss: 2.8190
    Epoch 43/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2.1935 - val_loss: 2.7392
    Epoch 44/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2.0877 - val_loss: 2.6569
    Epoch 45/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2.0413 - val_loss: 2.6212
    Epoch 46/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1.9730 - val_loss: 2.5352
    Epoch 47/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1.9038 - val_loss: 2.4922
    Epoch 48/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1.8635 - val_loss: 2.4479
    Epoch 49/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1.7839 - val_loss: 2.3742
    Epoch 50/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1.7329 - val_loss: 2.3278
    Epoch 51/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1.6863 - val_loss: 2.2540
    Epoch 52/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1.6281 - val_loss: 2.1972
    Epoch 53/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1.5721 - val_loss: 2.1973
    Epoch 54/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1.5472 - val_loss: 2.0886
    Epoch 55/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1.4970 - val_loss: 2.0672
    Epoch 56/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1.4505 - val_loss: 2.0068
    Epoch 57/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1.4009 - val_loss: 1.9678
    Epoch 58/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1.3311 - val_loss: 1.9551
    Epoch 59/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1.2981 - val_loss: 1.8835
    Epoch 60/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1.2471 - val_loss: 1.8670
    Validation Loss for Interval 2:
    [1805.4129638671875, 873.4866943359375, 214.52151489257812, 74.54344177246094, 102.66649627685547, 55.385562896728516, 41.25425338745117, 27.0007266998291, 9.112757682800293, 12.845159530639648, 11.734489440917969, 7.505561828613281, 7.874143123626709, 7.010127544403076, 6.332950592041016, 6.493390083312988, 6.351007461547852, 6.001019477844238, 5.600288391113281, 5.4574456214904785, 5.286937236785889, 5.177671432495117, 4.903094291687012, 4.696807384490967, 4.606385707855225, 4.4718122482299805, 4.31842565536499, 4.121487140655518, 4.005917072296143, 3.831479072570801, 3.782179594039917, 3.6943883895874023, 3.6269922256469727, 3.455548048019409, 3.4372100830078125, 3.419604539871216, 3.3457438945770264, 3.279897689819336, 3.246047019958496, 3.213550567626953, 3.072458267211914, 2.8190112113952637, 2.7391791343688965, 2.656907081604004, 2.6211636066436768, 2.5352447032928467, 2.4921765327453613, 2.4478533267974854, 2.3741846084594727, 2.327793598175049, 2.2540125846862793, 2.197178840637207, 2.1973228454589844, 2.0886127948760986, 2.0671606063842773, 2.0068116188049316, 1.9678237438201904, 1.9551242589950562, 1.8835123777389526, 1.8669887781143188]
    ========================================
    Decoded Forecasts for Interval 2 (Forecast Date: 2007-01-01):
    PRCP: [9.843829 9.90868  9.998536 9.658782] (Average: 9.85)
    TAVG: [70.7287   70.3008   69.6535   69.700806] (Average: 70.10)
    TMAX: [77.53456 77.32013 77.01792 77.90183] (Average: 77.44)
    TMIN: [58.90956  58.29344  57.340813 57.216415] (Average: 57.94)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m3s[0m 62ms/step - loss: 2250.3052 - val_loss: 1168.7288
    Epoch 2/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 893.6672 - val_loss: 227.6610
    Epoch 3/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 144.9112 - val_loss: 39.5481
    Epoch 4/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 65.8501 - val_loss: 158.4411
    Epoch 5/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 133.2944 - val_loss: 63.6501
    Epoch 6/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 41.5435 - val_loss: 14.5563
    Epoch 7/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 15.0885 - val_loss: 25.9730
    Epoch 8/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 25.9216 - val_loss: 19.8540
    Epoch 9/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 18.0994 - val_loss: 7.1309
    Epoch 10/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 7.7444 - val_loss: 8.1750
    Epoch 11/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 8.5782 - val_loss: 10.7545
    Epoch 12/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 9.1929 - val_loss: 6.9165
    Epoch 13/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 6.3947 - val_loss: 5.2161
    Epoch 14/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 6.0817 - val_loss: 5.9502
    Epoch 15/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 6.0768 - val_loss: 5.5748
    Epoch 16/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 5.4054 - val_loss: 4.9888
    Epoch 17/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 5.4740 - val_loss: 5.2718
    Epoch 18/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 5.3156 - val_loss: 4.9553
    Epoch 19/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.0345 - val_loss: 4.5283
    Epoch 20/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 4.8409 - val_loss: 4.3665
    Epoch 21/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 4.6375 - val_loss: 4.3786
    Epoch 22/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 4.4722 - val_loss: 4.1227
    Epoch 23/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 4.3361 - val_loss: 3.9054
    Epoch 24/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 4.1784 - val_loss: 3.7908
    Epoch 25/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 3.9901 - val_loss: 3.4246
    Epoch 26/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 3.8548 - val_loss: 3.3877
    Epoch 27/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.7265 - val_loss: 3.1838
    Epoch 28/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.5992 - val_loss: 3.1609
    Epoch 29/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.4819 - val_loss: 2.8878
    Epoch 30/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.3540 - val_loss: 2.8559
    Epoch 31/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 3.2310 - val_loss: 2.6903
    Epoch 32/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.1328 - val_loss: 2.6309
    Epoch 33/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 3.0188 - val_loss: 2.4579
    Epoch 34/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 2.9105 - val_loss: 2.4280
    Epoch 35/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 2.8168 - val_loss: 2.3092
    Epoch 36/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2.7101 - val_loss: 2.2198
    Epoch 37/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 2.6529 - val_loss: 2.1883
    Epoch 38/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2.5261 - val_loss: 1.9796
    Epoch 39/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 2.4462 - val_loss: 1.9157
    Epoch 40/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2.3949 - val_loss: 1.8946
    Epoch 41/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 2.2909 - val_loss: 1.7963
    Epoch 42/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2.2312 - val_loss: 1.7664
    Epoch 43/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2.1850 - val_loss: 1.7015
    Epoch 44/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 2.1059 - val_loss: 1.6407
    Epoch 45/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 2.0206 - val_loss: 1.6141
    Epoch 46/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1.9716 - val_loss: 1.5399
    Epoch 47/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1.9190 - val_loss: 1.5343
    Epoch 48/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1.8597 - val_loss: 1.4786
    Epoch 49/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1.8119 - val_loss: 1.4363
    Epoch 50/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1.7632 - val_loss: 1.4230
    Epoch 51/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1.7221 - val_loss: 1.3552
    Epoch 52/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1.6637 - val_loss: 1.3308
    Epoch 53/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1.6312 - val_loss: 1.2990
    Epoch 54/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1.6062 - val_loss: 1.2597
    Epoch 55/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1.5543 - val_loss: 1.2234
    Epoch 56/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1.4996 - val_loss: 1.1884
    Epoch 57/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1.4702 - val_loss: 1.1766
    Epoch 58/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1.4175 - val_loss: 1.1129
    Epoch 59/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1.3902 - val_loss: 1.0979
    Epoch 60/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1.3343 - val_loss: 1.0579
    Validation Loss for Interval 3:
    [1168.728759765625, 227.6609649658203, 39.548099517822266, 158.44107055664062, 63.65012741088867, 14.556333541870117, 25.972963333129883, 19.854007720947266, 7.130904197692871, 8.174973487854004, 10.75452709197998, 6.916452407836914, 5.216054439544678, 5.95023250579834, 5.574779987335205, 4.988834381103516, 5.271757125854492, 4.955268383026123, 4.528331756591797, 4.366515159606934, 4.378599166870117, 4.122684001922607, 3.905428171157837, 3.7907943725585938, 3.42456316947937, 3.387669801712036, 3.1837568283081055, 3.1609129905700684, 2.887848377227783, 2.855914354324341, 2.6902551651000977, 2.6308722496032715, 2.4578776359558105, 2.4279537200927734, 2.309227466583252, 2.2198281288146973, 2.188319683074951, 1.9795877933502197, 1.9157333374023438, 1.8945543766021729, 1.796263337135315, 1.7664028406143188, 1.7015113830566406, 1.6407455205917358, 1.6141048669815063, 1.5398874282836914, 1.5343085527420044, 1.4785802364349365, 1.4362775087356567, 1.422987461090088, 1.3552225828170776, 1.3307769298553467, 1.2990002632141113, 1.259655237197876, 1.2233766317367554, 1.1884437799453735, 1.1766152381896973, 1.1129380464553833, 1.0979082584381104, 1.0578666925430298]
    ========================================
    Decoded Forecasts for Interval 3 (Forecast Date: 2008-01-01):
    PRCP: [9.901598 9.76251  9.777224] (Average: 9.81)
    TAVG: [68.66312 69.21742 69.15343] (Average: 69.01)
    TMAX: [78.53299 78.80658 78.77387] (Average: 78.70)
    TMIN: [56.29339  57.777523 57.624   ] (Average: 57.23)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m2s[0m 62ms/step - loss: 3390.1472 - val_loss: 2666.4075
    Epoch 2/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 2384.8528 - val_loss: 1853.0170
    Epoch 3/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1612.1813 - val_loss: 1055.0372
    Epoch 4/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 858.6653 - val_loss: 349.5077
    Epoch 5/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 236.0456 - val_loss: 15.7663
    Epoch 6/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 20.9574 - val_loss: 128.1381
    Epoch 7/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 129.9776 - val_loss: 116.8317
    Epoch 8/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 85.9574 - val_loss: 17.5810
    Epoch 9/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 15.0221 - val_loss: 17.3434
    Epoch 10/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 23.3166 - val_loss: 27.2029
    Epoch 11/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 24.7199 - val_loss: 16.4709
    Epoch 12/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 11.7213 - val_loss: 12.7826
    Epoch 13/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 9.0347 - val_loss: 12.5727
    Epoch 14/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 10.3786 - val_loss: 8.3980
    Epoch 15/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 8.6229 - val_loss: 6.3510
    Epoch 16/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 7.2732 - val_loss: 8.3979
    Epoch 17/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 7.1641 - val_loss: 8.5614
    Epoch 18/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 6.8698 - val_loss: 7.8589
    Epoch 19/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 6.6866 - val_loss: 7.4726
    Epoch 20/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 6.5545 - val_loss: 7.4082
    Epoch 21/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 6.4893 - val_loss: 7.0495
    Epoch 22/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 6.3432 - val_loss: 7.0295
    Epoch 23/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 6.2220 - val_loss: 7.3006
    Epoch 24/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 6.1308 - val_loss: 7.1531
    Epoch 25/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 5.9656 - val_loss: 6.8106
    Epoch 26/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 5.7229 - val_loss: 6.8135
    Epoch 27/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 5.4052 - val_loss: 6.6142
    Epoch 28/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 5.1415 - val_loss: 6.3685
    Epoch 29/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 4.8326 - val_loss: 5.8477
    Epoch 30/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 4.4509 - val_loss: 5.1981
    Epoch 31/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 4.1369 - val_loss: 5.1172
    Epoch 32/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.8330 - val_loss: 5.0553
    Epoch 33/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 3.7866 - val_loss: 5.0083
    Epoch 34/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.5122 - val_loss: 4.6705
    Epoch 35/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.4070 - val_loss: 4.5756
    Epoch 36/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.2498 - val_loss: 4.3113
    Epoch 37/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 3.0872 - val_loss: 4.2677
    Epoch 38/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 2.9842 - val_loss: 4.0286
    Epoch 39/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 2.8258 - val_loss: 3.8693
    Epoch 40/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2.6913 - val_loss: 3.7765
    Epoch 41/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2.5771 - val_loss: 3.6724
    Epoch 42/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 2.4742 - val_loss: 3.4865
    Epoch 43/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2.3762 - val_loss: 3.3072
    Epoch 44/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 2.2453 - val_loss: 3.1755
    Epoch 45/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 2.1874 - val_loss: 3.0579
    Epoch 46/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 2.0659 - val_loss: 2.8449
    Epoch 47/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1.9905 - val_loss: 2.6954
    Epoch 48/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1.9143 - val_loss: 2.6077
    Epoch 49/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1.7911 - val_loss: 2.4018
    Epoch 50/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1.6618 - val_loss: 2.1460
    Epoch 51/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1.5884 - val_loss: 2.0236
    Epoch 52/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1.5129 - val_loss: 1.9154
    Epoch 53/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1.3798 - val_loss: 1.6955
    Epoch 54/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1.3231 - val_loss: 1.6457
    Epoch 55/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1.2558 - val_loss: 1.5938
    Epoch 56/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1.1900 - val_loss: 1.4033
    Epoch 57/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1.1565 - val_loss: 1.4335
    Epoch 58/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 1.0814 - val_loss: 1.2842
    Epoch 59/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 12ms/step - loss: 1.0443 - val_loss: 1.2011
    Epoch 60/60
    [1m5/5[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 8ms/step - loss: 0.9978 - val_loss: 1.1419
    Validation Loss for Interval 4:
    [2666.407470703125, 1853.0169677734375, 1055.0372314453125, 349.5076599121094, 15.766312599182129, 128.1381378173828, 116.8316879272461, 17.581008911132812, 17.34343910217285, 27.20290184020996, 16.47092628479004, 12.78257942199707, 12.572725296020508, 8.398015022277832, 6.351007461547852, 8.397889137268066, 8.561408996582031, 7.8589253425598145, 7.472640037536621, 7.408161640167236, 7.049526691436768, 7.029545783996582, 7.30057430267334, 7.153050422668457, 6.8105621337890625, 6.81349515914917, 6.614185333251953, 6.368486404418945, 5.847692489624023, 5.198086738586426, 5.117201328277588, 5.055340766906738, 5.008328437805176, 4.670478343963623, 4.575636863708496, 4.31131649017334, 4.267740726470947, 4.0285515785217285, 3.869253635406494, 3.7764780521392822, 3.6724131107330322, 3.4865000247955322, 3.3071508407592773, 3.1754777431488037, 3.057893753051758, 2.8448562622070312, 2.6953864097595215, 2.6077423095703125, 2.4018049240112305, 2.145981550216675, 2.02360200881958, 1.91543447971344, 1.695481300354004, 1.6457295417785645, 1.5938459634780884, 1.4032952785491943, 1.4334636926651, 1.284164547920227, 1.2011195421218872, 1.141853928565979]
    ========================================
    Decoded Forecasts for Interval 4 (Forecast Date: 2009-01-01):
    PRCP: [9.409122 9.331293 8.737331 9.128778 9.068665 8.810375] (Average: 9.08)
    TAVG: [69.594536 69.83923  67.93322  65.43776  65.634186 66.362404] (Average: 67.47)
    TMAX: [81.773865 81.760185 75.75721  75.45957  75.4288   75.287895] (Average: 77.58)
    TMIN: [56.712658 57.27512  56.813007 54.051617 54.52229  56.25717 ] (Average: 55.94)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m2s[0m 78ms/step - loss: 3083.3047 - val_loss: 2604.0330
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2321.2625 - val_loss: 1956.4916
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 1722.4552 - val_loss: 1347.7135
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 1151.3441 - val_loss: 761.4781
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 621.6992 - val_loss: 304.5405
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 238.5269 - val_loss: 81.5926
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 81.7772 - val_loss: 76.5800
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 89.7053 - val_loss: 101.2393
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 91.3985 - val_loss: 66.3207
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 49.9976 - val_loss: 35.7517
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 26.3607 - val_loss: 34.8410
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 27.8492 - val_loss: 35.3238
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 26.8040 - val_loss: 23.8505
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 16.6150 - val_loss: 11.5348
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 8.5396 - val_loss: 8.3339
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 8.8908 - val_loss: 9.8769
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 10.5181 - val_loss: 8.8508
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 8.7930 - val_loss: 7.3016
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.9782 - val_loss: 7.7551
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.7690 - val_loss: 9.1408
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 7.1450 - val_loss: 9.5480
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 7.0873 - val_loss: 8.9240
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.7481 - val_loss: 8.1840
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.6405 - val_loss: 7.7270
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.6122 - val_loss: 7.5431
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.5528 - val_loss: 7.5724
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.5021 - val_loss: 7.6701
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 6.4879 - val_loss: 7.6866
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.4563 - val_loss: 7.6298
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.4193 - val_loss: 7.5733
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.3845 - val_loss: 7.5813
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.3746 - val_loss: 7.6136
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.3626 - val_loss: 7.6024
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.3408 - val_loss: 7.5453
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.3336 - val_loss: 7.4752
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.3208 - val_loss: 7.4412
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.3037 - val_loss: 7.4491
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.2901 - val_loss: 7.4550
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.2675 - val_loss: 7.4305
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.2465 - val_loss: 7.3838
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 6.2510 - val_loss: 7.3643
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.2231 - val_loss: 7.3656
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.2079 - val_loss: 7.3385
    Epoch 44/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.1879 - val_loss: 7.2949
    Epoch 45/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.1784 - val_loss: 7.2700
    Epoch 46/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.1671 - val_loss: 7.2663
    Epoch 47/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.1438 - val_loss: 7.2554
    Epoch 48/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.1314 - val_loss: 7.2294
    Epoch 49/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.1109 - val_loss: 7.1937
    Epoch 50/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.0856 - val_loss: 7.1450
    Epoch 51/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.0755 - val_loss: 7.1029
    Epoch 52/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.0545 - val_loss: 7.0805
    Epoch 53/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.0188 - val_loss: 7.0668
    Epoch 54/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.0047 - val_loss: 7.0298
    Epoch 55/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.9680 - val_loss: 6.9780
    Epoch 56/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.9427 - val_loss: 6.9283
    Epoch 57/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.9146 - val_loss: 6.8799
    Epoch 58/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.8863 - val_loss: 6.8443
    Epoch 59/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.8247 - val_loss: 6.7138
    Epoch 60/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.7903 - val_loss: 6.5417
    Validation Loss for Interval 5:
    [2604.032958984375, 1956.4915771484375, 1347.7135009765625, 761.4781494140625, 304.54052734375, 81.5926284790039, 76.57998657226562, 101.2392807006836, 66.32068634033203, 35.751705169677734, 34.840972900390625, 35.32376480102539, 23.850536346435547, 11.534832954406738, 8.333877563476562, 9.87693977355957, 8.850790023803711, 7.301582336425781, 7.755095481872559, 9.140795707702637, 9.547975540161133, 8.924026489257812, 8.183985710144043, 7.727004528045654, 7.543087959289551, 7.57242488861084, 7.670113563537598, 7.686638832092285, 7.62976598739624, 7.573290824890137, 7.581342697143555, 7.613563537597656, 7.602379322052002, 7.5453314781188965, 7.475228786468506, 7.441161155700684, 7.449108600616455, 7.454983234405518, 7.430524826049805, 7.383820533752441, 7.364287853240967, 7.365574359893799, 7.338510036468506, 7.294857025146484, 7.269984722137451, 7.266310214996338, 7.255409240722656, 7.229377746582031, 7.193667888641357, 7.14502477645874, 7.102870464324951, 7.080523490905762, 7.06682825088501, 7.029809951782227, 6.977992057800293, 6.928274154663086, 6.879944324493408, 6.8442535400390625, 6.713771820068359, 6.541658878326416]
    ========================================
    Decoded Forecasts for Interval 5 (Forecast Date: 2010-01-01):
    PRCP: [4.258846  4.347324  4.3211293 4.143669 ] (Average: 4.27)
    TAVG: [65.872   70.32375 70.12094 68.78802] (Average: 68.78)
    TMAX: [76.75716  81.18855  80.95647  79.423935] (Average: 79.58)
    TMIN: [54.382057 58.056488 57.888283 56.78547 ] (Average: 56.78)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m2s[0m 68ms/step - loss: 3117.5710 - val_loss: 2613.2952
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 2344.8123 - val_loss: 1852.8452
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 1613.4209 - val_loss: 1151.1316
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 951.4113 - val_loss: 526.8748
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 390.6905 - val_loss: 114.5722
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 69.9817 - val_loss: 38.4177
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 55.7378 - val_loss: 134.2434
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 135.7382 - val_loss: 119.7380
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 100.9497 - val_loss: 41.3193
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 32.0487 - val_loss: 13.9290
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 13.4691 - val_loss: 23.1837
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 20.9750 - val_loss: 27.9596
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 23.0869 - val_loss: 23.3348
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 16.2996 - val_loss: 15.9792
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 9.0428 - val_loss: 11.0580
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.5439 - val_loss: 9.8889
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 7.5898 - val_loss: 9.1872
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 7.8276 - val_loss: 7.2968
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.3801 - val_loss: 6.5338
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.2611 - val_loss: 7.7206
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.3089 - val_loss: 8.5020
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.3423 - val_loss: 7.6961
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.9510 - val_loss: 6.5636
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.7573 - val_loss: 5.9936
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.7711 - val_loss: 5.8643
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.7074 - val_loss: 5.9799
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.5256 - val_loss: 6.0134
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.4155 - val_loss: 5.9244
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.3640 - val_loss: 5.7172
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.2702 - val_loss: 5.5355
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.1615 - val_loss: 5.3872
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.0736 - val_loss: 5.1794
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.0361 - val_loss: 4.9027
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.9531 - val_loss: 4.8943
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.8696 - val_loss: 5.0519
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.7810 - val_loss: 4.8315
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.7266 - val_loss: 4.5136
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.6436 - val_loss: 4.4192
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.5542 - val_loss: 4.4065
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.4705 - val_loss: 4.2678
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.3888 - val_loss: 4.0842
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.3128 - val_loss: 3.9290
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.2334 - val_loss: 3.7747
    Epoch 44/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.1382 - val_loss: 3.6952
    Epoch 45/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.0561 - val_loss: 3.5581
    Epoch 46/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 2.9774 - val_loss: 3.3490
    Epoch 47/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 2.8746 - val_loss: 3.2304
    Epoch 48/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 2.7849 - val_loss: 3.1355
    Epoch 49/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 2.6931 - val_loss: 2.9986
    Epoch 50/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2.6015 - val_loss: 2.9297
    Epoch 51/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2.5297 - val_loss: 2.7557
    Epoch 52/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 2.4621 - val_loss: 2.6252
    Epoch 53/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 2.4040 - val_loss: 2.5054
    Epoch 54/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2.3184 - val_loss: 2.3888
    Epoch 55/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2.2569 - val_loss: 2.2974
    Epoch 56/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 2.1732 - val_loss: 2.1587
    Epoch 57/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2.1052 - val_loss: 2.0803
    Epoch 58/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 2.0241 - val_loss: 1.9759
    Epoch 59/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1.9492 - val_loss: 1.7919
    Epoch 60/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1.8875 - val_loss: 1.7298
    Validation Loss for Interval 6:
    [2613.295166015625, 1852.84521484375, 1151.131591796875, 526.874755859375, 114.57223510742188, 38.41769027709961, 134.24339294433594, 119.73796081542969, 41.319305419921875, 13.92896842956543, 23.18367576599121, 27.959577560424805, 23.33475112915039, 15.979236602783203, 11.057987213134766, 9.888861656188965, 9.187186241149902, 7.296801567077637, 6.533812522888184, 7.720609664916992, 8.501965522766113, 7.696056842803955, 6.563584804534912, 5.993640422821045, 5.864319801330566, 5.979934215545654, 6.013439178466797, 5.924440383911133, 5.717202186584473, 5.535500526428223, 5.387235641479492, 5.179396629333496, 4.902724742889404, 4.894329071044922, 5.051863670349121, 4.8315019607543945, 4.513571739196777, 4.419236183166504, 4.406464099884033, 4.267824172973633, 4.084211349487305, 3.928971767425537, 3.774705648422241, 3.6952481269836426, 3.558135747909546, 3.349031448364258, 3.2304294109344482, 3.1355183124542236, 2.9986135959625244, 2.9297423362731934, 2.755706548690796, 2.625234842300415, 2.5053858757019043, 2.38875150680542, 2.297433853149414, 2.1586551666259766, 2.08034086227417, 1.9759252071380615, 1.7918699979782104, 1.72981858253479]
    ========================================
    Decoded Forecasts for Interval 6 (Forecast Date: 2011-01-01):
    PRCP: [7.0812874 7.1748486 7.345955 ] (Average: 7.20)
    TAVG: [69.717804 70.169556 69.777985] (Average: 69.89)
    TMAX: [81.31557 80.71744 78.83818] (Average: 80.29)
    TMIN: [57.862877 58.733955 58.898937] (Average: 58.50)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m3s[0m 83ms/step - loss: 3475.6506 - val_loss: 2703.8525
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 2326.1475 - val_loss: 1685.9447
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 1386.4254 - val_loss: 826.4341
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 610.1961 - val_loss: 224.5156
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 127.1472 - val_loss: 8.8335
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 29.7834 - val_loss: 106.3102
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 140.8294 - val_loss: 119.0265
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 118.7303 - val_loss: 38.8032
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 35.1631 - val_loss: 14.7074
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 12.4701 - val_loss: 30.8564
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 22.8239 - val_loss: 36.2003
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 24.3195 - val_loss: 23.8541
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 14.6573 - val_loss: 10.5539
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 7.3094 - val_loss: 6.2639
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 7.3407 - val_loss: 7.7028
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 9.2831 - val_loss: 8.3650
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 8.3824 - val_loss: 7.6393
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.1952 - val_loss: 7.8496
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.5811 - val_loss: 8.3910
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.8302 - val_loss: 7.8059
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.4949 - val_loss: 6.8408
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.1835 - val_loss: 6.5050
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.3426 - val_loss: 6.4359
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.4005 - val_loss: 6.3820
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 5.1841 - val_loss: 6.4113
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.0203 - val_loss: 6.4090
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.9504 - val_loss: 6.2722
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.9219 - val_loss: 6.1526
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.8941 - val_loss: 6.0980
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.8884 - val_loss: 6.0074
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.8379 - val_loss: 5.9308
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.7152 - val_loss: 5.8713
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.6477 - val_loss: 5.6402
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.6283 - val_loss: 5.7929
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.5826 - val_loss: 5.7046
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.5083 - val_loss: 5.4211
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.4859 - val_loss: 5.3073
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.4288 - val_loss: 5.3229
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.3654 - val_loss: 5.2849
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.2875 - val_loss: 5.0413
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.2242 - val_loss: 4.7641
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.1482 - val_loss: 4.6739
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.1014 - val_loss: 4.6610
    Epoch 44/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.0062 - val_loss: 4.5416
    Epoch 45/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.9424 - val_loss: 4.4027
    Epoch 46/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.8965 - val_loss: 4.3182
    Epoch 47/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.8271 - val_loss: 4.2401
    Epoch 48/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.7575 - val_loss: 4.1396
    Epoch 49/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.6808 - val_loss: 4.0301
    Epoch 50/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.6090 - val_loss: 3.9035
    Epoch 51/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.5805 - val_loss: 3.8367
    Epoch 52/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.5055 - val_loss: 3.7559
    Epoch 53/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.4554 - val_loss: 3.6585
    Epoch 54/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.4140 - val_loss: 3.5013
    Epoch 55/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.3440 - val_loss: 3.4023
    Epoch 56/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.2902 - val_loss: 3.3381
    Epoch 57/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.2499 - val_loss: 3.2761
    Epoch 58/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3.1808 - val_loss: 3.1479
    Epoch 59/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.1183 - val_loss: 3.0190
    Epoch 60/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.0908 - val_loss: 2.9520
    Validation Loss for Interval 7:
    [2703.8525390625, 1685.9447021484375, 826.4341430664062, 224.51556396484375, 8.83346939086914, 106.31016540527344, 119.02647399902344, 38.80323791503906, 14.707382202148438, 30.8564395904541, 36.20029067993164, 23.854055404663086, 10.553865432739258, 6.263852596282959, 7.702832221984863, 8.365026473999023, 7.6392974853515625, 7.849617958068848, 8.390987396240234, 7.805936813354492, 6.840822696685791, 6.504954814910889, 6.43588399887085, 6.381975173950195, 6.411253929138184, 6.409018039703369, 6.272175312042236, 6.1525726318359375, 6.097976207733154, 6.007425785064697, 5.930778980255127, 5.871327877044678, 5.640156269073486, 5.792890548706055, 5.704647541046143, 5.421140193939209, 5.307292461395264, 5.32293176651001, 5.2849345207214355, 5.041294574737549, 4.764138698577881, 4.673886299133301, 4.661004543304443, 4.541626930236816, 4.402717590332031, 4.31823205947876, 4.240070819854736, 4.139649391174316, 4.030066967010498, 3.9035229682922363, 3.8366916179656982, 3.755854368209839, 3.6584630012512207, 3.5013086795806885, 3.4022955894470215, 3.3381199836730957, 3.276087999343872, 3.1479222774505615, 3.0189738273620605, 2.951950788497925]
    ========================================
    Decoded Forecasts for Interval 7 (Forecast Date: 2012-01-01):
    PRCP: [7.32409   7.370213  7.2489023 7.2301903] (Average: 7.29)
    TAVG: [69.06781 68.45838 69.95463 69.8662 ] (Average: 69.34)
    TMAX: [78.24506 77.36625 79.54036 79.43213] (Average: 78.65)
    TMIN: [56.629032 56.241783 57.228157 56.95461 ] (Average: 56.76)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m2s[0m 83ms/step - loss: 3332.1140 - val_loss: 2835.0005
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 2617.2012 - val_loss: 2129.0081
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 1937.4315 - val_loss: 1419.7771
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1269.5828 - val_loss: 768.5445
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 667.8988 - val_loss: 283.0243
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 236.0316 - val_loss: 82.0088
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 74.2879 - val_loss: 119.6224
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 98.4518 - val_loss: 138.1802
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 96.6805 - val_loss: 72.1898
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 46.4781 - val_loss: 29.8223
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 24.1312 - val_loss: 28.0902
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 27.4198 - val_loss: 29.4469
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 26.0521 - val_loss: 19.9881
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 15.1126 - val_loss: 11.9789
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 7.8337 - val_loss: 13.2612
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 8.8631 - val_loss: 16.6109
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 10.7555 - val_loss: 15.8898
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 9.3150 - val_loss: 13.4251
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 7.4960 - val_loss: 12.0899
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 7.2868 - val_loss: 11.2214
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 7.2877 - val_loss: 10.4122
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 7.0068 - val_loss: 10.4214
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 6.8407 - val_loss: 11.2006
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.8740 - val_loss: 11.7820
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.8046 - val_loss: 11.6418
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.6869 - val_loss: 11.0651
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.6298 - val_loss: 10.5337
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.5969 - val_loss: 10.3680
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.5695 - val_loss: 10.5314
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.5379 - val_loss: 10.6793
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.4890 - val_loss: 10.6306
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.4314 - val_loss: 10.4979
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.4110 - val_loss: 10.4063
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.3967 - val_loss: 10.3361
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.3609 - val_loss: 10.2613
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.3238 - val_loss: 10.2020
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.3356 - val_loss: 10.1272
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 6.2226 - val_loss: 8.6617
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.1526 - val_loss: 10.0866
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.9627 - val_loss: 9.9920
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.8682 - val_loss: 9.3822
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 11ms/step - loss: 5.8207 - val_loss: 9.2773
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.6955 - val_loss: 8.9022
    Epoch 44/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.5728 - val_loss: 8.8372
    Epoch 45/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.4648 - val_loss: 8.9539
    Epoch 46/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.3437 - val_loss: 8.6663
    Epoch 47/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.2245 - val_loss: 8.4850
    Epoch 48/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.1379 - val_loss: 8.3849
    Epoch 49/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.0362 - val_loss: 7.9314
    Epoch 50/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.9715 - val_loss: 7.6638
    Epoch 51/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.8939 - val_loss: 7.8504
    Epoch 52/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.7775 - val_loss: 7.6276
    Epoch 53/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 4.6762 - val_loss: 7.2116
    Epoch 54/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.5611 - val_loss: 7.1488
    Epoch 55/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.3955 - val_loss: 6.5542
    Epoch 56/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.2911 - val_loss: 6.0925
    Epoch 57/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.1582 - val_loss: 6.2401
    Epoch 58/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.0404 - val_loss: 6.0004
    Epoch 59/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.9488 - val_loss: 5.7308
    Epoch 60/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.8304 - val_loss: 5.3903
    Validation Loss for Interval 8:
    [2835.00048828125, 2129.008056640625, 1419.777099609375, 768.5444946289062, 283.0242919921875, 82.0087661743164, 119.62242889404297, 138.18020629882812, 72.18981170654297, 29.822341918945312, 28.090177536010742, 29.4468994140625, 19.988094329833984, 11.978860855102539, 13.261157035827637, 16.610857009887695, 15.889799118041992, 13.425138473510742, 12.089911460876465, 11.221437454223633, 10.412169456481934, 10.421420097351074, 11.200592041015625, 11.782002449035645, 11.641772270202637, 11.065071105957031, 10.533700942993164, 10.367958068847656, 10.53136157989502, 10.679255485534668, 10.63062858581543, 10.497926712036133, 10.406316757202148, 10.336149215698242, 10.261250495910645, 10.201955795288086, 10.12723445892334, 8.66170597076416, 10.08655834197998, 9.99202823638916, 9.382173538208008, 9.277297973632812, 8.902212142944336, 8.837213516235352, 8.953930854797363, 8.666319847106934, 8.48497486114502, 8.38485336303711, 7.931392192840576, 7.663795471191406, 7.850430965423584, 7.6275787353515625, 7.211635112762451, 7.148812294006348, 6.554233074188232, 6.092495918273926, 6.240092754364014, 6.0004072189331055, 5.7307820320129395, 5.3902716636657715]
    ========================================
    Decoded Forecasts for Interval 8 (Forecast Date: 2013-01-01):
    PRCP: [5.8479915] (Average: 5.85)
    TAVG: [70.38917] (Average: 70.39)
    TMAX: [81.91001] (Average: 81.91)
    TMIN: [57.132362] (Average: 57.13)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m2s[0m 78ms/step - loss: 4274.0859 - val_loss: 3512.3557
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 3224.8875 - val_loss: 2649.4343
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2419.9949 - val_loss: 1964.1289
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 1785.8547 - val_loss: 1345.9290
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 1192.0798 - val_loss: 727.9202
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 619.2948 - val_loss: 264.0238
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 215.9369 - val_loss: 69.8737
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 68.1278 - val_loss: 81.3637
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 77.6176 - val_loss: 108.8202
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 86.3117 - val_loss: 86.9428
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 61.6060 - val_loss: 54.9115
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 37.9365 - val_loss: 31.5814
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 21.8190 - val_loss: 15.9961
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 11.7828 - val_loss: 11.9619
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 10.5334 - val_loss: 15.7432
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 13.5558 - val_loss: 17.0268
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 12.5921 - val_loss: 13.1383
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 8.1396 - val_loss: 10.4728
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.9183 - val_loss: 11.1064
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.4099 - val_loss: 11.9431
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.6193 - val_loss: 11.6900
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.0962 - val_loss: 11.1668
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.7798 - val_loss: 10.6469
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.8270 - val_loss: 10.1137
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.7543 - val_loss: 9.8385
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.7323 - val_loss: 9.8676
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.6754 - val_loss: 9.9977
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.5258 - val_loss: 9.9842
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.4489 - val_loss: 10.1575
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.4766 - val_loss: 10.2485
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.4220 - val_loss: 10.0801
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.3911 - val_loss: 9.8485
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.3757 - val_loss: 9.7624
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.3710 - val_loss: 9.8151
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.4000 - val_loss: 9.8442
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.3407 - val_loss: 9.7966
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.3154 - val_loss: 9.7205
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.3059 - val_loss: 9.6734
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.2697 - val_loss: 9.6657
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.2932 - val_loss: 9.6397
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.2586 - val_loss: 9.5759
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.2254 - val_loss: 9.4878
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.2456 - val_loss: 9.4563
    Epoch 44/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.2019 - val_loss: 9.4477
    Epoch 45/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.1728 - val_loss: 9.4165
    Epoch 46/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.1621 - val_loss: 9.3728
    Epoch 47/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.1653 - val_loss: 9.3058
    Epoch 48/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.1341 - val_loss: 9.2921
    Epoch 49/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.0974 - val_loss: 9.4556
    Epoch 50/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.0807 - val_loss: 8.6582
    Epoch 51/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.9973 - val_loss: 8.6952
    Epoch 52/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.9804 - val_loss: 8.4141
    Epoch 53/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.9429 - val_loss: 8.7532
    Epoch 54/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.9547 - val_loss: 8.7771
    Epoch 55/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.8893 - val_loss: 8.4955
    Epoch 56/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.8461 - val_loss: 8.3420
    Epoch 57/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 4.7737 - val_loss: 8.0579
    Epoch 58/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.5941 - val_loss: 8.2449
    Epoch 59/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.5683 - val_loss: 8.1435
    Epoch 60/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.5704 - val_loss: 8.1198
    Validation Loss for Interval 9:
    [3512.355712890625, 2649.434326171875, 1964.12890625, 1345.928955078125, 727.9202270507812, 264.0238342285156, 69.87369537353516, 81.36372375488281, 108.82022857666016, 86.94280242919922, 54.91148376464844, 31.58144760131836, 15.99614143371582, 11.961854934692383, 15.743163108825684, 17.026782989501953, 13.138309478759766, 10.472816467285156, 11.10635757446289, 11.943116188049316, 11.690028190612793, 11.166821479797363, 10.64692211151123, 10.11370849609375, 9.838536262512207, 9.867576599121094, 9.997681617736816, 9.984217643737793, 10.157503128051758, 10.248506546020508, 10.08005428314209, 9.848535537719727, 9.76242733001709, 9.815059661865234, 9.844216346740723, 9.79655933380127, 9.720515251159668, 9.673357963562012, 9.665714263916016, 9.639740943908691, 9.575850486755371, 9.487799644470215, 9.456345558166504, 9.44769287109375, 9.416459083557129, 9.372759819030762, 9.305790901184082, 9.292058944702148, 9.45556640625, 8.658195495605469, 8.69519329071045, 8.414063453674316, 8.753206253051758, 8.777145385742188, 8.495473861694336, 8.341951370239258, 8.057892799377441, 8.244922637939453, 8.143460273742676, 8.119800567626953]
    ========================================
    Decoded Forecasts for Interval 9 (Forecast Date: 2014-01-01):
    PRCP: [4.7597666 4.7685337 4.775249  4.805717 ] (Average: 4.78)
    TAVG: [70.40812  69.78222  68.93912  68.840675] (Average: 69.49)
    TMAX: [80.674545 80.10131  79.34561  79.14009 ] (Average: 79.82)
    TMIN: [58.82589  58.170094 57.300537 57.2406  ] (Average: 57.88)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m2s[0m 78ms/step - loss: 3515.9973 - val_loss: 2905.4031
    Epoch 2/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 2667.7097 - val_loss: 2066.6658
    Epoch 3/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 1866.1925 - val_loss: 1302.4968
    Epoch 4/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1144.9282 - val_loss: 648.7977
    Epoch 5/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 552.7530 - val_loss: 204.6998
    Epoch 6/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 167.5830 - val_loss: 35.0117
    Epoch 7/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 39.4147 - val_loss: 82.3273
    Epoch 8/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 82.9588 - val_loss: 125.1463
    Epoch 9/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 100.2184 - val_loss: 86.8023
    Epoch 10/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 59.2208 - val_loss: 41.3442
    Epoch 11/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 26.5106 - val_loss: 24.0985
    Epoch 12/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 19.3033 - val_loss: 20.2016
    Epoch 13/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 18.4166 - val_loss: 17.1198
    Epoch 14/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 14.7469 - val_loss: 15.6819
    Epoch 15/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 11.1758 - val_loss: 16.2726
    Epoch 16/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 9.5515 - val_loss: 15.6506
    Epoch 17/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 8.2637 - val_loss: 13.1886
    Epoch 18/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.9755 - val_loss: 11.2472
    Epoch 19/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.6217 - val_loss: 10.7036
    Epoch 20/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 6.5583 - val_loss: 11.0927
    Epoch 21/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.3704 - val_loss: 11.7881
    Epoch 22/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.2083 - val_loss: 12.0812
    Epoch 23/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.1055 - val_loss: 11.6362
    Epoch 24/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.9522 - val_loss: 10.8678
    Epoch 25/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.7818 - val_loss: 10.4040
    Epoch 26/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.7203 - val_loss: 10.4073
    Epoch 27/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.7010 - val_loss: 10.6157
    Epoch 28/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.7001 - val_loss: 10.7935
    Epoch 29/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.7116 - val_loss: 10.8628
    Epoch 30/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.7565 - val_loss: 10.8228
    Epoch 31/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.7679 - val_loss: 10.7148
    Epoch 32/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.6957 - val_loss: 10.6057
    Epoch 33/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.6716 - val_loss: 10.5297
    Epoch 34/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.6541 - val_loss: 10.5209
    Epoch 35/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.6356 - val_loss: 10.5633
    Epoch 36/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.6534 - val_loss: 10.6020
    Epoch 37/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.6382 - val_loss: 10.5954
    Epoch 38/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.6290 - val_loss: 10.5542
    Epoch 39/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.6243 - val_loss: 10.5048
    Epoch 40/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.6202 - val_loss: 10.4676
    Epoch 41/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.5986 - val_loss: 10.4555
    Epoch 42/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.5761 - val_loss: 10.4446
    Epoch 43/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.5826 - val_loss: 10.4325
    Epoch 44/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.5782 - val_loss: 10.4175
    Epoch 45/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.5701 - val_loss: 10.3906
    Epoch 46/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.5589 - val_loss: 10.3553
    Epoch 47/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.5570 - val_loss: 10.3420
    Epoch 48/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.5475 - val_loss: 10.3342
    Epoch 49/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 5.5220 - val_loss: 10.3152
    Epoch 50/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.5089 - val_loss: 10.2890
    Epoch 51/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.5054 - val_loss: 10.2666
    Epoch 52/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.5068 - val_loss: 10.2511
    Epoch 53/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.4889 - val_loss: 10.2275
    Epoch 54/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 21ms/step - loss: 5.4806 - val_loss: 10.1935
    Epoch 55/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.4654 - val_loss: 10.1682
    Epoch 56/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.4560 - val_loss: 10.1589
    Epoch 57/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 10ms/step - loss: 5.4343 - val_loss: 10.1525
    Epoch 58/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.4388 - val_loss: 10.1259
    Epoch 59/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.4115 - val_loss: 10.0770
    Epoch 60/60
    [1m4/4[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.3997 - val_loss: 10.0357
    Validation Loss for Interval 10:
    [2905.403076171875, 2066.665771484375, 1302.496826171875, 648.7977294921875, 204.6997528076172, 35.011661529541016, 82.32730102539062, 125.14631652832031, 86.80233764648438, 41.34423828125, 24.098491668701172, 20.201648712158203, 17.11983299255371, 15.681934356689453, 16.27257537841797, 15.650582313537598, 13.188581466674805, 11.247243881225586, 10.703595161437988, 11.092672348022461, 11.788089752197266, 12.081164360046387, 11.636192321777344, 10.867757797241211, 10.404007911682129, 10.407317161560059, 10.615653038024902, 10.793481826782227, 10.862767219543457, 10.822807312011719, 10.714836120605469, 10.605688095092773, 10.529671669006348, 10.52090072631836, 10.56328010559082, 10.6019868850708, 10.595354080200195, 10.554216384887695, 10.50478744506836, 10.467597961425781, 10.455489158630371, 10.444646835327148, 10.432470321655273, 10.417536735534668, 10.390583038330078, 10.355268478393555, 10.342013359069824, 10.334192276000977, 10.315204620361328, 10.289039611816406, 10.266590118408203, 10.251102447509766, 10.227527618408203, 10.193453788757324, 10.168240547180176, 10.158904075622559, 10.1525297164917, 10.125855445861816, 10.07699966430664, 10.03569507598877]
    ========================================
    Decoded Forecasts for Interval 10 (Forecast Date: 2015-01-01):
    PRCP: [4.2031584 4.1997457 4.2188225 4.176451 ] (Average: 4.20)
    TAVG: [72.21861 71.86882 71.55728 70.33923] (Average: 71.50)
    TMAX: [82.91452  82.521416 82.05756  80.6235  ] (Average: 82.03)
    TMIN: [59.58936  59.371876 59.251053 58.483128] (Average: 59.17)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m3s[0m 117ms/step - loss: 3243.1355 - val_loss: 2878.3748
    Epoch 2/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 2736.0938 - val_loss: 2408.3977
    Epoch 3/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2269.2456 - val_loss: 1939.7687
    Epoch 4/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1803.2157 - val_loss: 1452.5557
    Epoch 5/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1319.2904 - val_loss: 950.5935
    Epoch 6/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 833.0782 - val_loss: 486.9062
    Epoch 7/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 400.7907 - val_loss: 150.9261
    Epoch 8/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 108.1955 - val_loss: 14.2892
    Epoch 9/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 19.7468 - val_loss: 74.3336
    Epoch 10/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 92.6151 - val_loss: 152.6136
    Epoch 11/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 147.3747 - val_loss: 128.1136
    Epoch 12/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 107.3748 - val_loss: 61.7180
    Epoch 13/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 43.0974 - val_loss: 23.7191
    Epoch 14/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 12.5665 - val_loss: 21.5877
    Epoch 15/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 14.9914 - val_loss: 30.2681
    Epoch 16/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 24.9224 - val_loss: 32.1202
    Epoch 17/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 27.1278 - val_loss: 24.7360
    Epoch 18/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 20.9239 - val_loss: 14.8026
    Epoch 19/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 12.5368 - val_loss: 9.3108
    Epoch 20/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 8.0100 - val_loss: 9.7875
    Epoch 21/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 7.9360 - val_loss: 12.6326
    Epoch 22/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 9.0761 - val_loss: 13.9574
    Epoch 23/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 9.1210 - val_loss: 13.0472
    Epoch 24/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 7.7401 - val_loss: 11.4818
    Epoch 25/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.7742 - val_loss: 10.4448
    Epoch 26/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.6106 - val_loss: 9.9351
    Epoch 27/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.8180 - val_loss: 9.5806
    Epoch 28/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.7555 - val_loss: 9.2416
    Epoch 29/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.5149 - val_loss: 9.1847
    Epoch 30/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.2937 - val_loss: 9.4634
    Epoch 31/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.2221 - val_loss: 9.7897
    Epoch 32/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.2429 - val_loss: 9.8958
    Epoch 33/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.1777 - val_loss: 9.7576
    Epoch 34/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.0963 - val_loss: 9.5231
    Epoch 35/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.0518 - val_loss: 9.3231
    Epoch 36/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.0753 - val_loss: 9.2028
    Epoch 37/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.1002 - val_loss: 9.1730
    Epoch 38/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.0602 - val_loss: 9.2258
    Epoch 39/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.0296 - val_loss: 9.3228
    Epoch 40/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.0289 - val_loss: 9.3934
    Epoch 41/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.0068 - val_loss: 9.3920
    Epoch 42/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.0111 - val_loss: 9.3252
    Epoch 43/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.9947 - val_loss: 9.2318
    Epoch 44/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.9572 - val_loss: 9.1652
    Epoch 45/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.9756 - val_loss: 9.1384
    Epoch 46/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.9732 - val_loss: 9.1432
    Epoch 47/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.9397 - val_loss: 9.1610
    Epoch 48/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.9314 - val_loss: 9.1709
    Epoch 49/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.9239 - val_loss: 9.1638
    Epoch 50/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.9295 - val_loss: 9.1403
    Epoch 51/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.9080 - val_loss: 9.1084
    Epoch 52/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.8976 - val_loss: 9.0775
    Epoch 53/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.8876 - val_loss: 9.0537
    Epoch 54/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.8891 - val_loss: 9.0351
    Epoch 55/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.8831 - val_loss: 9.0255
    Epoch 56/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.8597 - val_loss: 9.0169
    Epoch 57/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.8642 - val_loss: 9.0076
    Epoch 58/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.8466 - val_loss: 8.9922
    Epoch 59/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.8292 - val_loss: 8.9720
    Epoch 60/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.8344 - val_loss: 8.9430
    Validation Loss for Interval 11:
    [2878.374755859375, 2408.397705078125, 1939.7686767578125, 1452.5556640625, 950.593505859375, 486.9062194824219, 150.92611694335938, 14.289153099060059, 74.33358764648438, 152.61361694335938, 128.1136474609375, 61.718040466308594, 23.71912956237793, 21.587671279907227, 30.26805305480957, 32.12019348144531, 24.736003875732422, 14.80258846282959, 9.310783386230469, 9.787520408630371, 12.63260555267334, 13.957415580749512, 13.047203063964844, 11.481780052185059, 10.444803237915039, 9.935128211975098, 9.580641746520996, 9.241613388061523, 9.184673309326172, 9.463408470153809, 9.789676666259766, 9.895792007446289, 9.757600784301758, 9.523070335388184, 9.323064804077148, 9.20277214050293, 9.173011779785156, 9.225824356079102, 9.322848320007324, 9.393448829650879, 9.39199161529541, 9.32521915435791, 9.231756210327148, 9.165234565734863, 9.13835620880127, 9.143158912658691, 9.161026954650879, 9.170930862426758, 9.163819313049316, 9.140307426452637, 9.108362197875977, 9.07750415802002, 9.053666114807129, 9.03514575958252, 9.025546073913574, 9.016913414001465, 9.007628440856934, 8.992241859436035, 8.971989631652832, 8.942956924438477]
    ========================================
    Decoded Forecasts for Interval 11 (Forecast Date: 2016-01-01):
    PRCP: [4.729837] (Average: 4.73)
    TAVG: [68.897865] (Average: 68.90)
    TMAX: [79.33633] (Average: 79.34)
    TMIN: [57.186672] (Average: 57.19)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m2s[0m 117ms/step - loss: 2596.5349 - val_loss: 2227.7695
    Epoch 2/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2081.4019 - val_loss: 1737.3726
    Epoch 3/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1608.3645 - val_loss: 1240.1531
    Epoch 4/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 1133.5327 - val_loss: 764.0049
    Epoch 5/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 686.3505 - val_loss: 362.1408
    Epoch 6/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 315.5249 - val_loss: 90.5498
    Epoch 7/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 77.5997 - val_loss: 5.9133
    Epoch 8/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 17.7100 - val_loss: 83.7479
    Epoch 9/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 85.7099 - val_loss: 160.2056
    Epoch 10/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 132.2657 - val_loss: 134.0803
    Epoch 11/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 95.5858 - val_loss: 60.2874
    Epoch 12/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 36.2400 - val_loss: 13.9390
    Epoch 13/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 9.5716 - val_loss: 6.1625
    Epoch 14/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 13.0529 - val_loss: 12.6643
    Epoch 15/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 22.2502 - val_loss: 14.5174
    Epoch 16/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 21.9844 - val_loss: 10.1806
    Epoch 17/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 14.1070 - val_loss: 7.5972
    Epoch 18/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 7.8037 - val_loss: 9.8334
    Epoch 19/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.6089 - val_loss: 11.9083
    Epoch 20/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.9442 - val_loss: 10.8744
    Epoch 21/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.5893 - val_loss: 8.1115
    Epoch 22/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.8974 - val_loss: 5.8286
    Epoch 23/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.5782 - val_loss: 4.7286
    Epoch 24/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.6481 - val_loss: 4.3116
    Epoch 25/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.4594 - val_loss: 4.2495
    Epoch 26/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 20ms/step - loss: 5.0525 - val_loss: 4.6405
    Epoch 27/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.7510 - val_loss: 5.3530
    Epoch 28/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 4.7307 - val_loss: 5.8728
    Epoch 29/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.6856 - val_loss: 5.8062
    Epoch 30/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 4.5258 - val_loss: 5.2972
    Epoch 31/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.3824 - val_loss: 4.7240
    Epoch 32/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 4.4408 - val_loss: 4.3203
    Epoch 33/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.4781 - val_loss: 4.1139
    Epoch 34/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.4589 - val_loss: 4.2467
    Epoch 35/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.3271 - val_loss: 4.5426
    Epoch 36/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 4.2582 - val_loss: 4.6681
    Epoch 37/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 4.1650 - val_loss: 4.5745
    Epoch 38/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 4.1214 - val_loss: 4.3893
    Epoch 39/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 4.0568 - val_loss: 4.2192
    Epoch 40/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.9976 - val_loss: 4.0730
    Epoch 41/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.9306 - val_loss: 4.0030
    Epoch 42/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.8306 - val_loss: 3.9577
    Epoch 43/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 3.7774 - val_loss: 3.8347
    Epoch 44/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 3.7830 - val_loss: 3.7068
    Epoch 45/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 3.7337 - val_loss: 3.6276
    Epoch 46/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.6726 - val_loss: 3.7228
    Epoch 47/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 3.5987 - val_loss: 3.1284
    Epoch 48/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 3.5775 - val_loss: 3.0315
    Epoch 49/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 3.5680 - val_loss: 3.5658
    Epoch 50/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 3.3645 - val_loss: 3.0552
    Epoch 51/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.2347 - val_loss: 2.6441
    Epoch 52/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 3.2250 - val_loss: 3.0317
    Epoch 53/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.1733 - val_loss: 2.9040
    Epoch 54/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 3.1129 - val_loss: 2.4642
    Epoch 55/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.0686 - val_loss: 2.6090
    Epoch 56/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 3.0109 - val_loss: 2.6440
    Epoch 57/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2.9413 - val_loss: 2.3768
    Epoch 58/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2.9292 - val_loss: 2.3650
    Epoch 59/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 2.8527 - val_loss: 2.4096
    Epoch 60/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2.8179 - val_loss: 2.2284
    Validation Loss for Interval 12:
    [2227.76953125, 1737.37255859375, 1240.153076171875, 764.0049438476562, 362.1408386230469, 90.54983520507812, 5.913276195526123, 83.74789428710938, 160.20562744140625, 134.080322265625, 60.28742599487305, 13.938956260681152, 6.162546157836914, 12.66430950164795, 14.517355918884277, 10.180618286132812, 7.597241401672363, 9.833393096923828, 11.9083251953125, 10.874403953552246, 8.111547470092773, 5.828649520874023, 4.728648662567139, 4.311646938323975, 4.249479293823242, 4.640498638153076, 5.352958679199219, 5.8727827072143555, 5.806191921234131, 5.297165393829346, 4.723959922790527, 4.320267200469971, 4.113940715789795, 4.246671676635742, 4.542602062225342, 4.668076038360596, 4.574496269226074, 4.389305114746094, 4.219211101531982, 4.072991371154785, 4.002963066101074, 3.9576921463012695, 3.8346633911132812, 3.7068252563476562, 3.627573251724243, 3.7228012084960938, 3.1283986568450928, 3.031526803970337, 3.5657997131347656, 3.0552167892456055, 2.644132137298584, 3.031738042831421, 2.904014825820923, 2.4642372131347656, 2.609013319015503, 2.644028663635254, 2.3768346309661865, 2.365037679672241, 2.4095771312713623, 2.2283620834350586]
    ========================================
    Decoded Forecasts for Interval 12 (Forecast Date: 2017-01-01):
    PRCP: [8.800148 9.522375 8.511267] (Average: 8.94)
    TAVG: [69.83364  70.28022  69.675446] (Average: 69.93)
    TMAX: [80.24253 80.72518 80.06872] (Average: 80.35)
    TMIN: [58.163376 59.34004  57.76873 ] (Average: 58.42)
    ========================================
    Epoch 1/60
    

    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\reshaping\flatten.py:37: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(**kwargs)
    C:\Users\EZEKIEL\anaconda3\Lib\site-packages\keras\src\layers\core\dense.py:87: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
      super().__init__(activity_regularizer=activity_regularizer, **kwargs)
    

    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m2s[0m 117ms/step - loss: 3442.9050 - val_loss: 2872.4153
    Epoch 2/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 2651.5530 - val_loss: 2133.0410
    Epoch 3/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1960.9587 - val_loss: 1445.9901
    Epoch 4/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 1323.7494 - val_loss: 856.9252
    Epoch 5/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 776.0685 - val_loss: 379.8141
    Epoch 6/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 337.6899 - val_loss: 83.1614
    Epoch 7/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 74.9547 - val_loss: 27.4679
    Epoch 8/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 31.8813 - val_loss: 131.7303
    Epoch 9/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 115.0437 - val_loss: 191.3393
    Epoch 10/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 148.3153 - val_loss: 136.5558
    Epoch 11/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 96.7359 - val_loss: 54.9949
    Epoch 12/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 37.5652 - val_loss: 15.2993
    Epoch 13/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 18.3559 - val_loss: 14.0308
    Epoch 14/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 26.1633 - val_loss: 20.1369
    Epoch 15/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 32.5746 - val_loss: 17.6922
    Epoch 16/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 27.0666 - val_loss: 10.8775
    Epoch 17/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 16.7014 - val_loss: 9.1707
    Epoch 18/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 10.9342 - val_loss: 13.6502
    Epoch 19/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 11.1293 - val_loss: 17.7151
    Epoch 20/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 12.2809 - val_loss: 16.4649
    Epoch 21/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 10.9408 - val_loss: 11.5520
    Epoch 22/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 8.5446 - val_loss: 7.1966
    Epoch 23/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 7.4615 - val_loss: 5.2112
    Epoch 24/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 8.0695 - val_loss: 4.6817
    Epoch 25/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 8.5251 - val_loss: 4.5521
    Epoch 26/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 8.2117 - val_loss: 4.8219
    Epoch 27/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 7.4335 - val_loss: 5.7665
    Epoch 28/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 7.0066 - val_loss: 6.9836
    Epoch 29/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.9941 - val_loss: 7.6554
    Epoch 30/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 7.1063 - val_loss: 7.4239
    Epoch 31/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.9664 - val_loss: 6.6618
    Epoch 32/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.8054 - val_loss: 5.8090
    Epoch 33/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.7873 - val_loss: 5.2137
    Epoch 34/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.7988 - val_loss: 5.0514
    Epoch 35/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.8099 - val_loss: 5.2459
    Epoch 36/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.6738 - val_loss: 5.6059
    Epoch 37/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.6173 - val_loss: 5.8968
    Epoch 38/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.5453 - val_loss: 5.9615
    Epoch 39/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.5539 - val_loss: 5.8248
    Epoch 40/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.5563 - val_loss: 5.6303
    Epoch 41/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.5508 - val_loss: 5.4792
    Epoch 42/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.4640 - val_loss: 5.4096
    Epoch 43/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.4083 - val_loss: 5.4268
    Epoch 44/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.3639 - val_loss: 5.2758
    Epoch 45/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.3501 - val_loss: 5.1261
    Epoch 46/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 27ms/step - loss: 6.2210 - val_loss: 5.2221
    Epoch 47/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.1359 - val_loss: 5.4097
    Epoch 48/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 6.1554 - val_loss: 5.4209
    Epoch 49/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.1076 - val_loss: 5.2173
    Epoch 50/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.0742 - val_loss: 5.0390
    Epoch 51/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 31ms/step - loss: 6.0528 - val_loss: 5.0440
    Epoch 52/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.9835 - val_loss: 5.1447
    Epoch 53/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 6.0081 - val_loss: 5.1875
    Epoch 54/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.9544 - val_loss: 5.1431
    Epoch 55/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.9390 - val_loss: 5.0727
    Epoch 56/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.8847 - val_loss: 4.9944
    Epoch 57/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.8530 - val_loss: 4.9242
    Epoch 58/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.8591 - val_loss: 4.8813
    Epoch 59/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 16ms/step - loss: 5.7503 - val_loss: 4.8679
    Epoch 60/60
    [1m3/3[0m [32m━━━━━━━━━━━━━━━━━━━━[0m[37m[0m [1m0s[0m 23ms/step - loss: 5.6867 - val_loss: 4.8801
    Validation Loss for Interval 13:
    [2872.415283203125, 2133.041015625, 1445.9901123046875, 856.9252319335938, 379.8140563964844, 83.1613540649414, 27.467914581298828, 131.7303466796875, 191.3393096923828, 136.55577087402344, 54.99485397338867, 15.299337387084961, 14.030755043029785, 20.136892318725586, 17.69220733642578, 10.877484321594238, 9.170745849609375, 13.650158882141113, 17.715097427368164, 16.464859008789062, 11.552007675170898, 7.196641445159912, 5.211180210113525, 4.681670665740967, 4.552108287811279, 4.821927070617676, 5.766533374786377, 6.983586311340332, 7.65543794631958, 7.423883438110352, 6.661800384521484, 5.809006690979004, 5.2136664390563965, 5.051356792449951, 5.245903491973877, 5.6059441566467285, 5.896826267242432, 5.961517333984375, 5.824827671051025, 5.6302642822265625, 5.479175090789795, 5.409610271453857, 5.426753044128418, 5.275784969329834, 5.1260666847229, 5.222059726715088, 5.4096527099609375, 5.4209370613098145, 5.217339038848877, 5.0390191078186035, 5.044026851654053, 5.144681930541992, 5.18754243850708, 5.143059730529785, 5.0726752281188965, 4.994375705718994, 4.924191951751709, 4.881308555603027, 4.867898464202881, 4.8800554275512695]
    ========================================
    Decoded Forecasts for Interval 13 (Forecast Date: 2018-01-01):
    PRCP: [7.212475  7.2327967 6.878593  6.824383 ] (Average: 7.04)
    TAVG: [70.64815  71.102425 70.557755 68.5345  ] (Average: 70.21)
    TMAX: [80.61345  81.03964  80.569824 78.659035] (Average: 80.22)
    TMIN: [58.492092 58.814373 58.42024  56.959896] (Average: 58.17)
    ========================================
    


```python

```


```python

```


```python
# Generate synthetic data for the year 2019
# This is a placeholder. You need to replace this with your actual method of generating data.


# Preprocess the generated data
# Ensure it has the same format and shape as your historical data
data =pd.DataFrame(data)

# Use the trained autoencoder model to predict future weather for the year 2019
encoded_forecast_2019 = denoising_ae.layers[0](data.drop('DATE', axis=1).values)  # Access encoder layers
decoded_forecast_2019 = denoising_ae.layers[1](encoded_forecast_2019)  # Access decoder layers

# Store the decoded forecast results for the year 2019
forecast_results_2019 = decoded_forecast_2019

# Print or visualize the forecast results for the year 2019
print("Forecast Results for the Year 2019:")
print(forecast_results_2019)

```

    Forecast Results for the Year 2019:
    tf.Tensor(
    [[ 4.874032  65.795906  76.39676   54.87489  ]
     [ 6.005196  68.367355  78.65469   56.794453 ]
     [ 5.2926445 67.65132   78.22108   56.348724 ]
     [ 6.520949  68.97755   78.81027   57.00099  ]
     [ 5.411193  67.23865   77.3414    55.712803 ]
     [ 5.2115617 65.70071   75.43683   54.234707 ]
     [ 5.1424966 65.57884   75.33352   54.1468   ]
     [ 5.0771494 65.64987   75.47688   54.250973 ]
     [ 5.2030897 65.870316  75.66441   54.411243 ]
     [ 5.0475454 66.28402   76.93837   55.321888 ]
     [ 5.1423807 67.08779   77.6936    55.917416 ]
     [ 5.715108  67.74626   78.245186  56.43356  ]
     [ 5.039539  66.74559   77.41571   55.687366 ]
     [ 4.7424645 66.654205  77.86539   55.99412  ]
     [ 5.602895  68.10072   79.129135  57.111164 ]
     [ 6.964074  67.998985  77.92354   56.413387 ]
     [ 6.3531246 66.99646   77.086205  55.656025 ]
     [ 5.354661  63.545258  73.28812   52.54324  ]
     [ 4.4942074 60.501614  70.514175  50.289387 ]
     [ 4.5120564 60.531208  70.54007   50.312176 ]
     [ 4.527022  61.691822  71.65369   51.164433 ]
     [ 4.309234  63.924397  74.83757   53.53455  ]
     [ 5.422538  65.63646   76.36719   54.81261  ]
     [ 5.0145655 65.026024  75.821915  54.366993 ]
     [ 4.463222  64.16656   75.05268   53.719143 ]
     [ 4.3266244 64.33251   75.374794  53.935226 ]
     [ 4.3167725 64.316666  75.3604    53.92305  ]
     [ 5.233597  65.721664  76.619415  54.972427 ]
     [ 5.014018  65.394165  76.325455  54.7335   ]
     [ 4.9002867 65.2211    76.16974   54.60532  ]
     [ 4.2659245 64.23449   75.28563   53.859745 ]
     [ 4.3946133 64.5536    75.58324   54.10081  ]
     [ 4.334106  64.457634  75.496475  54.02738  ]
     [ 4.8586316 67.72894   78.76543   56.697063 ]
     [ 5.42297   67.70465   78.10234   56.282146 ]
     [ 5.0915666 67.16841   77.63963   55.872128 ]
     [ 5.2160916 67.90305   78.71939   56.721638 ]
     [ 4.789907  67.88612   79.02742   56.88959  ]
     [ 5.9618483 69.48054   80.26381   58.031593 ]
     [ 6.839922  68.98092   78.88578   57.14182  ]
     [ 5.56366   66.351204  76.42314   55.019375 ]
     [ 5.3325024 65.96004   76.08886   54.72035  ]
     [ 5.1874933 65.7214    75.88422   54.536854 ]
     [ 5.1812673 65.71135   75.875565  54.529087 ]
     [ 5.2229786 66.38164   76.72467   55.179283 ]
     [ 5.4106402 66.17029   76.486946  55.023197 ]
     [ 5.566165  66.018524  76.18742   54.819473 ]
     [ 5.7561045 66.59952   76.79911   55.32348  ]
     [ 5.93739   67.49422   77.62512   56.00237  ]
     [ 5.174671  67.22728   77.82448   56.022198 ]
     [ 5.3888884 68.05035   78.83209   56.837803 ]
     [ 6.5706744 69.92708   80.429565  58.264748 ]
     [ 6.6783295 67.84981   77.54283   56.093243 ]
     [ 5.2095065 64.93201   74.85417   53.7515   ]
     [ 5.494652  65.12501   74.86718   53.80473  ]
     [ 5.3529854 64.87877   74.65705   53.619843 ]
     [ 5.2740045 66.38989   76.77783   55.233707 ]
     [ 5.747889  66.43107   76.501755  55.099064 ]
     [ 6.1857643 67.409775  77.46889   55.910603 ]
     [ 5.0810075 65.65709   75.96125   54.57352  ]
     [ 5.1978574 66.10531   76.374374  54.912724 ]
     [ 6.309167  67.859055  77.866905  56.236393 ]
     [ 6.206856  67.70063   77.74055   56.120224 ]
     [ 9.002042  73.048     82.59919   59.95695  ]
     [ 4.910306  66.196365  76.50031   54.970226 ]
     [ 4.8793435 63.19118   73.61559   52.730457 ]
     [ 5.2882786 65.17173   75.46118   54.220257 ]
     [ 4.9461026 64.92343   75.386765  54.10712  ]
     [ 4.9664726 66.09221   76.5049    54.974766 ]
     [ 6.2153687 68.05977   78.20172   56.47101  ]
     [ 5.5794153 67.07998   77.35943   55.729404 ]
     [ 4.8864927 65.01616   75.484314  54.172176 ]
     [ 4.88773   65.132965  75.59598   54.258533 ]
     [ 5.589108  66.277466  76.59142   55.142456 ]
     [ 5.624297  67.54892   77.803055  56.075775 ]
     [ 6.5474014 68.936195  78.973045  57.09894  ]
     [ 4.9441676 64.62583   74.72333   53.601856 ]
     [ 4.961544  63.6352    73.39994   52.611874 ]
     [ 4.9764075 61.64994   71.514984  51.11762  ]
     [ 4.9405103 61.590553  71.46398   51.072186 ]
     [ 5.1997185 62.017982  71.83079   51.39918  ]
     [10.391128  71.68472   80.5235    58.030804 ]
     [ 5.673832  62.80131   72.502045  51.998116 ]
     [ 5.2221236 65.77165   76.7914    55.237236 ]
     [ 6.875677  70.61267   80.60052   58.42771  ]
     [ 6.3545218 69.080215  78.92781   57.090145 ]
     [ 4.8692517 64.19644   74.33525   53.28787  ]
     [ 5.1848755 63.758434  73.53319   52.735023 ]
     [ 5.0062103 63.204258  72.932205  52.251453 ]
     [ 4.6503496 63.462765  73.86337   52.889645 ]
     [ 4.9399714 63.94186   74.28232   53.259655 ]
     [ 5.323482  64.56776   74.828415  53.741676 ]
     [ 5.6902223 65.156265  75.340416  54.19209  ]
     [ 6.3327336 66.151794  76.17561   54.937748 ]
     [ 5.051503  64.12489   74.442184  53.400845 ]
     [ 4.779089  63.67638   74.05028   53.05469  ]
     [ 4.7117023 63.564697  73.95256   52.96842  ]
     [ 5.2813263 67.10362   77.512024  55.802486 ]
     [ 5.1845856 65.0206    75.00534   53.859097 ]
     [ 4.8963385 64.064255  73.950806  53.01802  ]
     [ 4.6568117 62.839314  73.0748    52.282772 ]
     [ 4.498706  63.75189   74.41356   53.289066 ]
     [ 5.0931816 66.21297   76.71188   55.107502 ]
     [ 5.1025147 66.51239   77.00119   55.318493 ]
     [ 5.563392  66.91711   77.06379   55.503773 ]
     [ 4.6993933 67.13263   77.96959   56.05399  ]
     [ 5.5162635 67.72218   78.55522   56.649372 ]
     [ 5.1237817 66.98212   77.867584  56.054012 ]
     [ 6.1870985 67.63364   77.932274  56.275936 ]
     [ 5.494281  65.54379   75.70088   54.431988 ]
     [ 5.320071  65.25929   75.456665  54.213375 ]
     [ 5.1117983 64.9172    75.16244   53.950413 ]
     [ 5.4310675 64.62419   74.53386   53.533432 ]
     [ 5.1608315 64.16179   74.13841   53.181232 ]
     [ 5.6418576 68.31146   78.74434   56.810352 ]
     [ 6.653284  68.502304  78.207565  56.549076 ]
     [ 5.2344856 66.12109   76.11832   54.74744  ]
     [ 5.239561  67.617516  78.08802   56.229404 ]
     [ 5.2024126 68.34351   79.099625  56.987125 ]
     [ 5.84343   69.324646  79.96585   57.72153  ]
     [ 5.365624  67.529434  77.885864  56.09658  ]
     [ 5.370864  67.71684   78.06553   56.234608 ]
     [ 5.2606106 66.96428   77.15223   55.52843  ]
     [ 5.1600685 65.43921   75.18339   54.03595  ]
     [ 5.1600685 65.43921   75.18339   54.03595  ]
     [ 5.061659  65.51724   76.054245  54.643787 ]
     [ 5.094651  65.47934   75.9789    54.59081  ]
     [ 4.9396567 65.22377   75.7558    54.393223 ]
     [ 4.991269  65.30904   75.83026   54.45917  ]
     [ 4.9206157 66.1253    76.97782   55.33368  ]
     [ 5.4649453 69.24997   80.087006  57.81707  ]
     [ 5.2136974 68.838196  79.72847   57.498318 ]
     [ 5.3970075 69.13904   79.99048   57.73127  ]
     [ 5.6635127 67.36626   77.44385   55.83182  ]
     [ 5.3601418 65.15086   74.869156  53.80845  ]
     [ 5.0209713 64.58796   74.38758   53.389156 ]
     [ 5.000569  64.55362   74.35829   53.363644 ]
     [ 4.904439  64.39668   74.223976  53.246323 ]
     [ 4.5841804 66.58979   77.37175   55.557125 ]
     [ 5.765558  66.84131   76.85602   55.34316  ]
     [ 4.843841  65.41244   75.61398   54.27157  ]
     [ 4.758085  65.274414  75.493805  54.166912 ]
     [ 4.7978563 67.4958    78.75539   56.685627 ]
     [ 5.114209  67.61506   78.6655    56.667034 ]
     [ 6.696673  70.19556   80.86842   58.638508 ]
     [ 6.521057  67.083664  76.85669   55.523495 ]
     [ 5.2988954 64.73726   74.739426  53.659542 ]
     [ 4.778224  62.83967   72.88182   52.152378 ]
     [ 4.836619  62.934803  72.96472   52.225426 ]
     [ 4.8083673 66.34008   77.07025   55.382442 ]
     [ 5.439177  67.37768   77.97546   56.18484  ]
     [ 7.269058  70.19472   80.38866   58.291065 ]
     [ 5.861866  69.862755  80.29371   58.00355  ]
     [ 7.4281225 72.20345   82.30495   59.738758 ]
     [ 6.084895  70.51674   80.88251   58.538895 ]
     [ 5.437932  69.487885  79.99273   57.756046 ]
     [ 5.825422  69.7579    80.05415   57.8769   ]
     [ 5.899582  69.09804   79.08842   57.147003 ]
     [ 5.88836   66.02786   76.193596  54.86715  ]
     [ 5.341407  65.131165  75.42778   54.17552  ]
     [ 5.1252794 66.354836  77.19404   55.523727 ]
     [ 5.1639853 66.112015  76.84172   55.25387  ]
     [ 5.099107  66.5242    77.439926  55.712147 ]
     [ 5.466945  64.56679   74.601036  53.567852 ]
     [ 5.272044  65.474625  75.91948   54.5488   ]
     [ 6.4997377 67.47258   77.62482   56.0937   ]
     [ 6.440976  67.766945  78.056274  56.418743 ]
     [ 6.224022  68.947655  79.79584   57.728897 ]
     [ 6.421566  67.86475   78.199776  56.52682  ]
     [ 6.4674807 70.17897   80.4       58.239365 ]
     [ 6.4465075 70.27081   80.541306  58.338856 ]
     [ 6.4577017 70.54236   80.79776   58.54028  ]
     [ 6.585268  69.77847   79.64238   57.691204 ]
     [ 6.5621524 67.96913   77.92815   56.35597  ]
     [ 6.575718  68.479034  78.41524   56.74166  ]
     [ 6.5859323 70.33725   80.17395   58.084503 ]
     [ 6.600229  70.16153   79.92458   57.88876  ]
     [ 6.612194  69.98361   79.67203   57.68885  ]
     [ 6.639905  69.33132   78.74111   56.94366  ]
     [ 6.1371737 67.71222   78.013     56.318893 ]
     [ 5.703559  68.83417   79.15263   57.102253 ]
     [ 5.7011027 68.7959    79.11608   57.074867 ]
     [ 5.5434985 70.12099   81.05795   58.485508 ]
     [ 6.7841225 69.56389   79.326904  57.431934 ]
     [ 6.8668895 68.67327   78.03313   56.435238 ]
     [ 5.1108546 68.29463   78.8921    56.83592  ]
     [ 5.1196947 68.24504   78.82124   56.78378  ]
     [ 6.8272095 70.12353   80.3534    58.20087  ]
     [ 7.0560665 68.643135  78.132996  56.577858 ]
     [ 6.9655113 69.20765   78.973724  57.19932  ]
     [ 5.7949266 69.45801   80.23777   57.960682 ]
     [ 5.886241  68.814545  79.29799   57.263462 ]
     [ 5.902885  69.2733    79.734055  57.59231  ]
     [ 5.971426  69.4129    79.98999   57.82236  ]
     [ 5.9742737 69.52815   80.09952   57.906338 ]
     [ 5.9784203 69.50333   80.06339   57.87939  ]
     [ 6.1092825 68.77191   78.7276    56.88167  ]
     [ 6.0016866 67.5274    77.506134  55.908566 ]
     [ 6.1190786 66.66671   76.21602   54.96037  ]
     [ 6.012718  69.745125  80.28253   58.05492  ]
     [ 6.96984   71.82603   82.10091   59.57775  ]
     [ 6.975374  71.97944   82.24721   59.686977 ]
     [ 7.1431603 70.90404   80.64177   58.50065  ]
     [ 7.12798   70.457886  80.21292   58.191814 ]
     [ 7.1005316 69.77813   79.557556  57.707558 ]
     [ 7.0451746 70.08156   80.017975  58.04102  ]
     [ 7.022869  69.35571   79.3428    57.514484 ]
     [ 7.0583725 70.42231   80.33605   58.285416 ]
     [ 7.0527687 70.30825   80.228745  58.203037 ]
     [ 6.881163  70.94324   81.36348   59.023724 ]
     [ 6.9018884 71.35594   81.75866   59.3142   ]
     [ 7.1799917 69.46307   78.94324   57.2207   ]
     [ 6.769561  66.900894  76.52975   55.242863 ]
     [ 6.781169  67.24541   76.85606   55.488514 ]
     [ 6.880272  68.52992   78.07364   56.42709  ]
     [ 6.8384986 68.02222   77.587616  56.057568 ]
     [ 7.0291615 71.87274   82.09235   59.59746  ]
     [ 7.017745  71.61166   81.84546   59.41638  ]
     [ 6.967762  69.86595   80.18651   58.161373 ]
     [ 6.993291  70.819046  81.0961    58.854977 ]
     [ 7.0109463 71.63194   81.8376    59.396206 ]
     [ 7.121621  71.001305  80.88385   58.706787 ]
     [ 7.3274374 71.317215  81.16095   58.9334   ]
     [ 7.372692  70.98158   80.67035   58.55844  ]
     [ 7.238179  71.810455  81.90263   59.474564 ]
     [ 7.2262707 71.505905  81.615685  59.25732  ]
     [ 7.1913557 70.45326   80.618805  58.515175 ]
     [ 7.2279654 71.54301   81.65074   59.28289  ]
     [ 7.199249  70.75662   80.90679   58.731968 ]
     [ 7.176009  69.68744   79.88835   57.960346 ]
     [ 7.2042923 69.49717   79.60666   57.747066 ]
     [ 7.1418524 73.095985  83.83584   60.97643  ]
     [ 7.1961184 72.77695   83.36946   60.631287 ]
     [ 7.2235937 72.548676  82.89476   60.238476 ]
     [ 7.2543516 71.48935   81.41294   59.09584  ]
     [ 7.173853  69.439026  79.47237   57.631668 ]
     [ 7.190588  70.12222   80.12096   58.121025 ]
     [ 7.2712407 71.79904   81.712234  59.32041  ]
     [ 7.1762595 69.553505  79.581345  57.714317 ]
     [ 7.212475  70.64815   80.61345   58.492092 ]
     [ 7.2327986 71.10243   81.03964   58.81438  ]
     [ 6.8785934 70.557755  80.569824  58.42024  ]
     [ 6.8243833 68.5345    78.65903   56.959892 ]], shape=(243, 4), dtype=float32)
    


```python

```


```python
import numpy as np
import pandas as pd

encoded_forecast_2019 = denoising_ae.layers[0](data.drop('DATE', axis=1).values)  # Access encoder layers
decoded_forecast_2019 = denoising_ae.layers[1](encoded_forecast_2019)  # Access decoder layers

# Store the decoded forecast results for the year 2019
forecast_results_2019 = decoded_forecast_2019

# Print or visualize the forecast results for the year 2019
print("Forecast Results for the Year 2019:")
print(forecast_results_2019)

# Convert TensorFlow tensor to NumPy array
forecast_results_np = forecast_results_2019.numpy()

# Calculate the mean average for each parameter
mean_averages = np.mean(forecast_results_np, axis=0)

# Print or visualize the mean averages for each parameter
print("Mean Averages for Forecast Data:")
print(mean_averages)

```

    Forecast Results for the Year 2019:
    tf.Tensor(
    [[ 4.874032  65.795906  76.39676   54.87489  ]
     [ 6.005196  68.367355  78.65469   56.794453 ]
     [ 5.2926445 67.65132   78.22108   56.348724 ]
     [ 6.520949  68.97755   78.81027   57.00099  ]
     [ 5.411193  67.23865   77.3414    55.712803 ]
     [ 5.2115617 65.70071   75.43683   54.234707 ]
     [ 5.1424966 65.57884   75.33352   54.1468   ]
     [ 5.0771494 65.64987   75.47688   54.250973 ]
     [ 5.2030897 65.870316  75.66441   54.411243 ]
     [ 5.0475454 66.28402   76.93837   55.321888 ]
     [ 5.1423807 67.08779   77.6936    55.917416 ]
     [ 5.715108  67.74626   78.245186  56.43356  ]
     [ 5.039539  66.74559   77.41571   55.687366 ]
     [ 4.7424645 66.654205  77.86539   55.99412  ]
     [ 5.602895  68.10072   79.129135  57.111164 ]
     [ 6.964074  67.998985  77.92354   56.413387 ]
     [ 6.3531246 66.99646   77.086205  55.656025 ]
     [ 5.354661  63.545258  73.28812   52.54324  ]
     [ 4.4942074 60.501614  70.514175  50.289387 ]
     [ 4.5120564 60.531208  70.54007   50.312176 ]
     [ 4.527022  61.691822  71.65369   51.164433 ]
     [ 4.309234  63.924397  74.83757   53.53455  ]
     [ 5.422538  65.63646   76.36719   54.81261  ]
     [ 5.0145655 65.026024  75.821915  54.366993 ]
     [ 4.463222  64.16656   75.05268   53.719143 ]
     [ 4.3266244 64.33251   75.374794  53.935226 ]
     [ 4.3167725 64.316666  75.3604    53.92305  ]
     [ 5.233597  65.721664  76.619415  54.972427 ]
     [ 5.014018  65.394165  76.325455  54.7335   ]
     [ 4.9002867 65.2211    76.16974   54.60532  ]
     [ 4.2659245 64.23449   75.28563   53.859745 ]
     [ 4.3946133 64.5536    75.58324   54.10081  ]
     [ 4.334106  64.457634  75.496475  54.02738  ]
     [ 4.8586316 67.72894   78.76543   56.697063 ]
     [ 5.42297   67.70465   78.10234   56.282146 ]
     [ 5.0915666 67.16841   77.63963   55.872128 ]
     [ 5.2160916 67.90305   78.71939   56.721638 ]
     [ 4.789907  67.88612   79.02742   56.88959  ]
     [ 5.9618483 69.48054   80.26381   58.031593 ]
     [ 6.839922  68.98092   78.88578   57.14182  ]
     [ 5.56366   66.351204  76.42314   55.019375 ]
     [ 5.3325024 65.96004   76.08886   54.72035  ]
     [ 5.1874933 65.7214    75.88422   54.536854 ]
     [ 5.1812673 65.71135   75.875565  54.529087 ]
     [ 5.2229786 66.38164   76.72467   55.179283 ]
     [ 5.4106402 66.17029   76.486946  55.023197 ]
     [ 5.566165  66.018524  76.18742   54.819473 ]
     [ 5.7561045 66.59952   76.79911   55.32348  ]
     [ 5.93739   67.49422   77.62512   56.00237  ]
     [ 5.174671  67.22728   77.82448   56.022198 ]
     [ 5.3888884 68.05035   78.83209   56.837803 ]
     [ 6.5706744 69.92708   80.429565  58.264748 ]
     [ 6.6783295 67.84981   77.54283   56.093243 ]
     [ 5.2095065 64.93201   74.85417   53.7515   ]
     [ 5.494652  65.12501   74.86718   53.80473  ]
     [ 5.3529854 64.87877   74.65705   53.619843 ]
     [ 5.2740045 66.38989   76.77783   55.233707 ]
     [ 5.747889  66.43107   76.501755  55.099064 ]
     [ 6.1857643 67.409775  77.46889   55.910603 ]
     [ 5.0810075 65.65709   75.96125   54.57352  ]
     [ 5.1978574 66.10531   76.374374  54.912724 ]
     [ 6.309167  67.859055  77.866905  56.236393 ]
     [ 6.206856  67.70063   77.74055   56.120224 ]
     [ 9.002042  73.048     82.59919   59.95695  ]
     [ 4.910306  66.196365  76.50031   54.970226 ]
     [ 4.8793435 63.19118   73.61559   52.730457 ]
     [ 5.2882786 65.17173   75.46118   54.220257 ]
     [ 4.9461026 64.92343   75.386765  54.10712  ]
     [ 4.9664726 66.09221   76.5049    54.974766 ]
     [ 6.2153687 68.05977   78.20172   56.47101  ]
     [ 5.5794153 67.07998   77.35943   55.729404 ]
     [ 4.8864927 65.01616   75.484314  54.172176 ]
     [ 4.88773   65.132965  75.59598   54.258533 ]
     [ 5.589108  66.277466  76.59142   55.142456 ]
     [ 5.624297  67.54892   77.803055  56.075775 ]
     [ 6.5474014 68.936195  78.973045  57.09894  ]
     [ 4.9441676 64.62583   74.72333   53.601856 ]
     [ 4.961544  63.6352    73.39994   52.611874 ]
     [ 4.9764075 61.64994   71.514984  51.11762  ]
     [ 4.9405103 61.590553  71.46398   51.072186 ]
     [ 5.1997185 62.017982  71.83079   51.39918  ]
     [10.391128  71.68472   80.5235    58.030804 ]
     [ 5.673832  62.80131   72.502045  51.998116 ]
     [ 5.2221236 65.77165   76.7914    55.237236 ]
     [ 6.875677  70.61267   80.60052   58.42771  ]
     [ 6.3545218 69.080215  78.92781   57.090145 ]
     [ 4.8692517 64.19644   74.33525   53.28787  ]
     [ 5.1848755 63.758434  73.53319   52.735023 ]
     [ 5.0062103 63.204258  72.932205  52.251453 ]
     [ 4.6503496 63.462765  73.86337   52.889645 ]
     [ 4.9399714 63.94186   74.28232   53.259655 ]
     [ 5.323482  64.56776   74.828415  53.741676 ]
     [ 5.6902223 65.156265  75.340416  54.19209  ]
     [ 6.3327336 66.151794  76.17561   54.937748 ]
     [ 5.051503  64.12489   74.442184  53.400845 ]
     [ 4.779089  63.67638   74.05028   53.05469  ]
     [ 4.7117023 63.564697  73.95256   52.96842  ]
     [ 5.2813263 67.10362   77.512024  55.802486 ]
     [ 5.1845856 65.0206    75.00534   53.859097 ]
     [ 4.8963385 64.064255  73.950806  53.01802  ]
     [ 4.6568117 62.839314  73.0748    52.282772 ]
     [ 4.498706  63.75189   74.41356   53.289066 ]
     [ 5.0931816 66.21297   76.71188   55.107502 ]
     [ 5.1025147 66.51239   77.00119   55.318493 ]
     [ 5.563392  66.91711   77.06379   55.503773 ]
     [ 4.6993933 67.13263   77.96959   56.05399  ]
     [ 5.5162635 67.72218   78.55522   56.649372 ]
     [ 5.1237817 66.98212   77.867584  56.054012 ]
     [ 6.1870985 67.63364   77.932274  56.275936 ]
     [ 5.494281  65.54379   75.70088   54.431988 ]
     [ 5.320071  65.25929   75.456665  54.213375 ]
     [ 5.1117983 64.9172    75.16244   53.950413 ]
     [ 5.4310675 64.62419   74.53386   53.533432 ]
     [ 5.1608315 64.16179   74.13841   53.181232 ]
     [ 5.6418576 68.31146   78.74434   56.810352 ]
     [ 6.653284  68.502304  78.207565  56.549076 ]
     [ 5.2344856 66.12109   76.11832   54.74744  ]
     [ 5.239561  67.617516  78.08802   56.229404 ]
     [ 5.2024126 68.34351   79.099625  56.987125 ]
     [ 5.84343   69.324646  79.96585   57.72153  ]
     [ 5.365624  67.529434  77.885864  56.09658  ]
     [ 5.370864  67.71684   78.06553   56.234608 ]
     [ 5.2606106 66.96428   77.15223   55.52843  ]
     [ 5.1600685 65.43921   75.18339   54.03595  ]
     [ 5.1600685 65.43921   75.18339   54.03595  ]
     [ 5.061659  65.51724   76.054245  54.643787 ]
     [ 5.094651  65.47934   75.9789    54.59081  ]
     [ 4.9396567 65.22377   75.7558    54.393223 ]
     [ 4.991269  65.30904   75.83026   54.45917  ]
     [ 4.9206157 66.1253    76.97782   55.33368  ]
     [ 5.4649453 69.24997   80.087006  57.81707  ]
     [ 5.2136974 68.838196  79.72847   57.498318 ]
     [ 5.3970075 69.13904   79.99048   57.73127  ]
     [ 5.6635127 67.36626   77.44385   55.83182  ]
     [ 5.3601418 65.15086   74.869156  53.80845  ]
     [ 5.0209713 64.58796   74.38758   53.389156 ]
     [ 5.000569  64.55362   74.35829   53.363644 ]
     [ 4.904439  64.39668   74.223976  53.246323 ]
     [ 4.5841804 66.58979   77.37175   55.557125 ]
     [ 5.765558  66.84131   76.85602   55.34316  ]
     [ 4.843841  65.41244   75.61398   54.27157  ]
     [ 4.758085  65.274414  75.493805  54.166912 ]
     [ 4.7978563 67.4958    78.75539   56.685627 ]
     [ 5.114209  67.61506   78.6655    56.667034 ]
     [ 6.696673  70.19556   80.86842   58.638508 ]
     [ 6.521057  67.083664  76.85669   55.523495 ]
     [ 5.2988954 64.73726   74.739426  53.659542 ]
     [ 4.778224  62.83967   72.88182   52.152378 ]
     [ 4.836619  62.934803  72.96472   52.225426 ]
     [ 4.8083673 66.34008   77.07025   55.382442 ]
     [ 5.439177  67.37768   77.97546   56.18484  ]
     [ 7.269058  70.19472   80.38866   58.291065 ]
     [ 5.861866  69.862755  80.29371   58.00355  ]
     [ 7.4281225 72.20345   82.30495   59.738758 ]
     [ 6.084895  70.51674   80.88251   58.538895 ]
     [ 5.437932  69.487885  79.99273   57.756046 ]
     [ 5.825422  69.7579    80.05415   57.8769   ]
     [ 5.899582  69.09804   79.08842   57.147003 ]
     [ 5.88836   66.02786   76.193596  54.86715  ]
     [ 5.341407  65.131165  75.42778   54.17552  ]
     [ 5.1252794 66.354836  77.19404   55.523727 ]
     [ 5.1639853 66.112015  76.84172   55.25387  ]
     [ 5.099107  66.5242    77.439926  55.712147 ]
     [ 5.466945  64.56679   74.601036  53.567852 ]
     [ 5.272044  65.474625  75.91948   54.5488   ]
     [ 6.4997377 67.47258   77.62482   56.0937   ]
     [ 6.440976  67.766945  78.056274  56.418743 ]
     [ 6.224022  68.947655  79.79584   57.728897 ]
     [ 6.421566  67.86475   78.199776  56.52682  ]
     [ 6.4674807 70.17897   80.4       58.239365 ]
     [ 6.4465075 70.27081   80.541306  58.338856 ]
     [ 6.4577017 70.54236   80.79776   58.54028  ]
     [ 6.585268  69.77847   79.64238   57.691204 ]
     [ 6.5621524 67.96913   77.92815   56.35597  ]
     [ 6.575718  68.479034  78.41524   56.74166  ]
     [ 6.5859323 70.33725   80.17395   58.084503 ]
     [ 6.600229  70.16153   79.92458   57.88876  ]
     [ 6.612194  69.98361   79.67203   57.68885  ]
     [ 6.639905  69.33132   78.74111   56.94366  ]
     [ 6.1371737 67.71222   78.013     56.318893 ]
     [ 5.703559  68.83417   79.15263   57.102253 ]
     [ 5.7011027 68.7959    79.11608   57.074867 ]
     [ 5.5434985 70.12099   81.05795   58.485508 ]
     [ 6.7841225 69.56389   79.326904  57.431934 ]
     [ 6.8668895 68.67327   78.03313   56.435238 ]
     [ 5.1108546 68.29463   78.8921    56.83592  ]
     [ 5.1196947 68.24504   78.82124   56.78378  ]
     [ 6.8272095 70.12353   80.3534    58.20087  ]
     [ 7.0560665 68.643135  78.132996  56.577858 ]
     [ 6.9655113 69.20765   78.973724  57.19932  ]
     [ 5.7949266 69.45801   80.23777   57.960682 ]
     [ 5.886241  68.814545  79.29799   57.263462 ]
     [ 5.902885  69.2733    79.734055  57.59231  ]
     [ 5.971426  69.4129    79.98999   57.82236  ]
     [ 5.9742737 69.52815   80.09952   57.906338 ]
     [ 5.9784203 69.50333   80.06339   57.87939  ]
     [ 6.1092825 68.77191   78.7276    56.88167  ]
     [ 6.0016866 67.5274    77.506134  55.908566 ]
     [ 6.1190786 66.66671   76.21602   54.96037  ]
     [ 6.012718  69.745125  80.28253   58.05492  ]
     [ 6.96984   71.82603   82.10091   59.57775  ]
     [ 6.975374  71.97944   82.24721   59.686977 ]
     [ 7.1431603 70.90404   80.64177   58.50065  ]
     [ 7.12798   70.457886  80.21292   58.191814 ]
     [ 7.1005316 69.77813   79.557556  57.707558 ]
     [ 7.0451746 70.08156   80.017975  58.04102  ]
     [ 7.022869  69.35571   79.3428    57.514484 ]
     [ 7.0583725 70.42231   80.33605   58.285416 ]
     [ 7.0527687 70.30825   80.228745  58.203037 ]
     [ 6.881163  70.94324   81.36348   59.023724 ]
     [ 6.9018884 71.35594   81.75866   59.3142   ]
     [ 7.1799917 69.46307   78.94324   57.2207   ]
     [ 6.769561  66.900894  76.52975   55.242863 ]
     [ 6.781169  67.24541   76.85606   55.488514 ]
     [ 6.880272  68.52992   78.07364   56.42709  ]
     [ 6.8384986 68.02222   77.587616  56.057568 ]
     [ 7.0291615 71.87274   82.09235   59.59746  ]
     [ 7.017745  71.61166   81.84546   59.41638  ]
     [ 6.967762  69.86595   80.18651   58.161373 ]
     [ 6.993291  70.819046  81.0961    58.854977 ]
     [ 7.0109463 71.63194   81.8376    59.396206 ]
     [ 7.121621  71.001305  80.88385   58.706787 ]
     [ 7.3274374 71.317215  81.16095   58.9334   ]
     [ 7.372692  70.98158   80.67035   58.55844  ]
     [ 7.238179  71.810455  81.90263   59.474564 ]
     [ 7.2262707 71.505905  81.615685  59.25732  ]
     [ 7.1913557 70.45326   80.618805  58.515175 ]
     [ 7.2279654 71.54301   81.65074   59.28289  ]
     [ 7.199249  70.75662   80.90679   58.731968 ]
     [ 7.176009  69.68744   79.88835   57.960346 ]
     [ 7.2042923 69.49717   79.60666   57.747066 ]
     [ 7.1418524 73.095985  83.83584   60.97643  ]
     [ 7.1961184 72.77695   83.36946   60.631287 ]
     [ 7.2235937 72.548676  82.89476   60.238476 ]
     [ 7.2543516 71.48935   81.41294   59.09584  ]
     [ 7.173853  69.439026  79.47237   57.631668 ]
     [ 7.190588  70.12222   80.12096   58.121025 ]
     [ 7.2712407 71.79904   81.712234  59.32041  ]
     [ 7.1762595 69.553505  79.581345  57.714317 ]
     [ 7.212475  70.64815   80.61345   58.492092 ]
     [ 7.2327986 71.10243   81.03964   58.81438  ]
     [ 6.8785934 70.557755  80.569824  58.42024  ]
     [ 6.8243833 68.5345    78.65903   56.959892 ]], shape=(243, 4), dtype=float32)
    Mean Averages for Forecast Data:
    [ 5.815758 67.394    77.63934  55.97619 ]
    


```python

```


```python

```


```python

```


```python
import pandas as pd
import numpy as np

# parameter names
parameter_names = ['PRCP', 'TAVG', 'TMAX', 'TMIN']


encoded_forecast_2019 = denoising_ae.layers[0](data.drop('DATE', axis=1).values)  # Access encoder layers
decoded_forecast_2019 = denoising_ae.layers[1](encoded_forecast_2019)  # Access decoder layers

# Create a DataFrame with the decoded forecast results and parameter names
forecast_results_df = pd.DataFrame(decoded_forecast_2019.numpy(), columns=parameter_names)

# Print or visualize the forecast results for the year 2019
print("Forecast Results for the Year 2019:")
print(forecast_results_df)

# Calculate the mean average for each parameter
mean_averages = forecast_results_df.mean()

# Print or visualize the mean averages for each parameter
print("Mean Averages for Forecast Data:")
print(mean_averages)

    
```

    Forecast Results for the Year 2019:
             PRCP       TAVG       TMAX       TMIN
    0    4.874032  65.795906  76.396759  54.874889
    1    6.005196  68.367355  78.654694  56.794453
    2    5.292645  67.651321  78.221077  56.348724
    3    6.520949  68.977547  78.810272  57.000992
    4    5.411193  67.238647  77.341400  55.712803
    ..        ...        ...        ...        ...
    238  7.176260  69.553505  79.581345  57.714317
    239  7.212475  70.648148  80.613449  58.492092
    240  7.232799  71.102432  81.039642  58.814381
    241  6.878593  70.557755  80.569824  58.420238
    242  6.824383  68.534500  78.659027  56.959892
    
    [243 rows x 4 columns]
    Mean Averages for Forecast Data:
    PRCP     5.815758
    TAVG    67.393997
    TMAX    77.639343
    TMIN    55.976189
    dtype: float32
    


```python
import pandas as pd
import numpy as np

# parameter names
parameter_names = ['PRCP', 'TAVG', 'TMAX', 'TMIN']

# Define the starting year and number of years to predict
start_year = 2019
num_years = 2  # Predict for 5 years (2019 to 2023)

# Iterate over each year and predict the weather
for year in range(start_year, start_year + num_years):
    # Generate synthetic data for the current year (replace this with your method)
    # For demonstration, let's assume random data is generated
    num_samples = 365  # Assuming one data point per day for the year
    num_features = len(parameter_names)
    synthetic_data = pd.DataFrame(np.random.rand(num_samples, num_features)*120,
                                  columns=parameter_names)
    synthetic_data['DATE'] = pd.date_range(start=f'{2019}-01-01', end=f'{2019}-12-31')
    
    # Use the trained autoencoder model to predict future weather for the current year
    encoded_forecast = denoising_ae.layers[0](synthetic_data.drop('DATE', axis=1).values)
    decoded_forecast = denoising_ae.layers[1](encoded_forecast)
    
    # Create a DataFrame with the decoded forecast results and parameter names
    forecast_results_df = pd.DataFrame(decoded_forecast.numpy(), columns=parameter_names)
    
    # Print or visualize the forecast results for the current year
    print(f"Forecast Results for the Year {year}:")
    print(forecast_results_df)
    
    # Calculate the mean average for each parameter
    mean_averages = forecast_results_df.mean()
    
    # Print or visualize the mean averages for each parameter
    print(f"Mean Averages for Forecast Data {year}:")
    print(mean_averages)

```

    Forecast Results for the Year 2019:
              PRCP       TAVG        TMAX       TMIN
    0    15.001297  97.990990  108.874786  80.313675
    1     8.081405  55.282173   45.433155  28.472404
    2    13.861498  81.633957   78.885567  52.665482
    3    12.728844  47.496731   52.510197  25.105661
    4    10.708144  59.807789   66.712639  47.716209
    ..         ...        ...         ...        ...
    360  13.026019  77.733246   84.400970  43.988468
    361  14.885337  96.750999   99.709961  57.671551
    362  19.417690  96.915268  104.713501  72.144081
    363  16.413399  83.494583   81.342621  48.785809
    364  15.005776  79.547699   83.274826  57.150558
    
    [365 rows x 4 columns]
    Mean Averages for Forecast Data 2019:
    PRCP    11.834857
    TAVG    74.393394
    TMAX    79.313629
    TMIN    53.163994
    dtype: float32
    Forecast Results for the Year 2020:
              PRCP        TAVG        TMAX       TMIN
    0    11.182754   67.018326   67.821701  48.308651
    1    12.941370   85.833199   95.089676  49.728603
    2    19.446510  106.094986  114.437988  81.532974
    3    15.883346   81.883499   84.918457  51.715328
    4    18.553726  101.498718  111.110649  79.403419
    ..         ...         ...         ...        ...
    360   7.773080   49.802128   50.871441  35.629330
    361   8.277238   65.840454   73.432037  41.593895
    362   8.164958   32.644012   35.662289  24.215607
    363  18.038296   90.124237   93.937691  68.951233
    364  18.614494   80.558159   87.412811  64.833061
    
    [365 rows x 4 columns]
    Mean Averages for Forecast Data 2020:
    PRCP    11.902569
    TAVG    74.004028
    TMAX    79.239273
    TMIN    53.190319
    dtype: float32
    


```python
import numpy as np
import pandas as pd

# Define the range of historical data for each parameter
historical_ranges = {
    "PRCP": (2.5, 10.75),    # Example historical range for precipitation (in mm)
    "TAVG": (67, 70),   # Example historical range for average temperature (in Celsius)
    "TMAX": (76, 83),   # Example historical range for maximum temperature (in Celsius)
    "TMIN": (56, 58)    # Example historical range for minimum temperature (in Celsius)
}

# Generate synthetic data
num_samples = 200000000  # Number of samples
num_features = len(historical_ranges)  # Number of features (parameters)

# Generate synthetic data using random values between 0 and 1
synthetic_data_normalized = pd.DataFrame(np.random.rand(num_samples, num_features),
                                          columns=list(historical_ranges.keys()))

# Scale synthetic data to match the range of historical data for each parameter
scaled_synthetic_data = pd.DataFrame()
for param in historical_ranges.keys():
    param_min, param_max = historical_ranges[param]
    scaled_synthetic_data[param] = synthetic_data_normalized[param] * (param_max - param_min) + param_min

# Print the scaled synthetic data
print("Scaled Synthetic Data:")
print(scaled_synthetic_data)

```

    Scaled Synthetic Data:
                   PRCP       TAVG       TMAX       TMIN
    0          5.183685  69.137864  81.717456  56.363228
    1          5.560263  69.705821  81.646855  57.969717
    2          8.722548  68.179586  80.134465  57.322029
    3          3.147260  68.633491  80.965246  56.334643
    4          8.940212  68.751318  82.665552  56.084845
    ...             ...        ...        ...        ...
    199999995  2.661751  69.596299  77.541298  57.937410
    199999996  7.421593  68.780846  82.627616  57.708394
    199999997  6.217301  69.018721  79.601356  56.294725
    199999998  5.659870  69.789504  79.752399  57.453043
    199999999  2.664377  67.726442  81.624689  56.892571
    
    [200000000 rows x 4 columns]
    


```python
import pandas as pd
import numpy as np

# parameter names
parameter_names = ['PRCP', 'TAVG', 'TMAX', 'TMIN']

# Define the starting year and number of years to predict
start_year = 2019
num_years = 2  # Predict for 5 years (2019 to 2023)

# Iterate over each year and predict the weather
for year in range(start_year, start_year + num_years):
    # Generate synthetic data for the current year (replace this with your method)
    # For demonstration, let's assume random data is generated
    num_samples = 365  # Assuming one data point per day for the year
    num_features = len(parameter_names)
    synthetic_data = pd.DataFrame(np.random.rand(num_samples, num_features)*120,
                                  columns=parameter_names)
    synthetic_data['DATE'] = pd.date_range(start=f'{2019}-01-01', end=f'{2019}-12-31')
    
    # Use the trained autoencoder model to predict future weather for the current year
    encoded_forecast = denoising_ae.layers[0](synthetic_data.drop('DATE', axis=1).values)
    decoded_forecast = denoising_ae.layers[1](encoded_forecast)
    
    # Create a DataFrame with the decoded forecast results and parameter names
    forecast_results_df = pd.DataFrame(decoded_forecast.numpy(), columns=parameter_names)
    
    # Print or visualize the forecast results for the current year
    print(f"Forecast Results for the Year {year}:")
    print(forecast_results_df)
    
    # Calculate the mean average for each parameter
    mean_averages = forecast_results_df.mean()
    
    # Print or visualize the mean averages for each parameter
    print(f"Mean Averages for Forecast Data {year}:")
    print(mean_averages)

```

    Forecast Results for the Year 2019:
              PRCP       TAVG        TMAX       TMIN
    0    16.253689  83.035507   85.061768  61.191002
    1     6.547073  85.683311   93.756485  68.057755
    2    10.184305  71.099747   72.804810  41.224026
    3    19.129871  78.081398   83.617729  59.322475
    4     4.732483  41.635120   48.151463  33.254238
    ..         ...        ...         ...        ...
    360  10.839050  62.143703   56.473835  32.552002
    361   8.833097  50.335461   55.911442  26.955669
    362  17.058819  95.166061  103.708725  75.742371
    363  11.820441  55.947887   60.394840  44.771244
    364   8.695275  45.669514   51.362381  36.908840
    
    [365 rows x 4 columns]
    Mean Averages for Forecast Data 2019:
    PRCP    11.768003
    TAVG    74.096481
    TMAX    79.310295
    TMIN    53.378162
    dtype: float32
    Forecast Results for the Year 2020:
              PRCP        TAVG        TMAX       TMIN
    0    12.538762   99.981163  107.380470  66.203514
    1    11.618697   77.770477   81.272041  54.385750
    2    10.529502  102.915192  108.559341  78.575775
    3     6.582004   43.838932   49.517120  27.002728
    4    19.966076   85.732468   93.345352  69.615219
    ..         ...         ...         ...        ...
    360  16.605509   63.593884   67.443245  40.145550
    361  11.637473   70.663315   78.992302  46.394268
    362   8.931206   71.105942   82.141754  58.307716
    363  17.317492  122.296013  134.838455  99.071342
    364  10.913480   59.802494   64.957382  39.875973
    
    [365 rows x 4 columns]
    Mean Averages for Forecast Data 2020:
    PRCP    11.576102
    TAVG    73.621170
    TMAX    79.168213
    TMIN    52.979023
    dtype: float32
    


```python
import numpy as np
import pandas as pd

# Define the range of historical data for each parameter
historical_ranges = {
    "PRCP": (2.5, 10.75),    # Example historical range for precipitation (in mm)
    "TAVG": (67, 70),   # Example historical range for average temperature (in Celsius)
    "TMAX": (76, 83),   # Example historical range for maximum temperature (in Celsius)
    "TMIN": (56, 58)    # Example historical range for minimum temperature (in Celsius)
}

# Generate synthetic data for each parameter separately
synthetic_data = {}
for param, (param_min, param_max) in historical_ranges.items():
    synthetic_data[param] = np.random.uniform(param_min, param_max, size=num_samples)

# Create a DataFrame from the synthetic data
synthetic_data_df = pd.DataFrame(synthetic_data)

# Print the synthetic data
print("Synthetic Data:")
print(synthetic_data_df)

```

    Synthetic Data:
              PRCP       TAVG       TMAX       TMIN
    0     7.900741  69.648322  76.568977  56.035690
    1     9.793180  68.041785  81.841714  57.294555
    2     8.351680  69.403491  77.713296  56.128799
    3     3.013268  67.048114  78.425908  57.187218
    4    10.463381  69.546814  81.408045  57.134969
    ..         ...        ...        ...        ...
    360   7.943068  69.515828  79.482190  57.773329
    361   5.183579  67.999902  79.430873  56.929865
    362   5.075888  67.348899  82.460883  57.448619
    363   8.441316  67.016524  77.961858  57.823649
    364   9.764395  68.914989  81.004317  57.911805
    
    [365 rows x 4 columns]
    


```python
import pandas as pd
import numpy as np

# parameter names
parameter_names = ['PRCP', 'TAVG', 'TMAX', 'TMIN']

# Define the starting year and number of years to predict
start_year = 2019
num_years = 2  # Predict for 5 years (2019 to 2023)

# Iterate over each year and predict the weather
for year in range(start_year, start_year + num_years):
    # Generate synthetic data for the current year (replace this with your method)
    # For demonstration, let's assume random data is generated
    num_samples = 365  # Assuming one data point per day for the year
    num_features = len(parameter_names)
    synthetic_data = pd.DataFrame(np.random.rand(num_samples, num_features)*120,
                                  columns=parameter_names)
    synthetic_data['DATE'] = pd.date_range(start=f'{2019}-01-01', end=f'{2019}-12-31')
    
    # Use the trained autoencoder model to predict future weather for the current year
    encoded_forecast = denoising_ae.layers[0](synthetic_data.drop('DATE', axis=1).values)
    decoded_forecast = denoising_ae.layers[1](encoded_forecast)
    
    # Create a DataFrame with the decoded forecast results and parameter names
    forecast_results_df = pd.DataFrame(decoded_forecast.numpy(), columns=parameter_names)
    
    # Print or visualize the forecast results for the current year
    print(f"Forecast Results for the Year {year}:")
    print(forecast_results_df)
    
    # Calculate the mean average for each parameter
    mean_averages = forecast_results_df.mean()
    
    # Print or visualize the mean averages for each parameter
    print(f" mean avarage for Forecast Data {year}:")
    print(mean_averages)

```

    Forecast Results for the Year 2019:
              PRCP        TAVG        TMAX       TMIN
    0    15.813964   63.843792   68.781860  50.575718
    1    17.282135   88.040543   94.603943  59.645451
    2    12.546805   82.843987   91.203156  48.086296
    3    10.029778  104.253448  110.524338  78.723022
    4    14.051291   83.078163   81.062744  45.109905
    ..         ...         ...         ...        ...
    360  19.930195  111.928787  122.600487  87.332306
    361  19.469473   87.391632   95.187912  70.622467
    362  18.660252   83.207642   91.699043  68.149109
    363  13.419137   75.403503   74.487846  44.584904
    364  20.410952  117.673088  130.178223  94.768494
    
    [365 rows x 4 columns]
     mean avarage for Forecast Data 2019:
    PRCP    12.324173
    TAVG    75.514839
    TMAX    80.706573
    TMIN    54.091850
    dtype: float32
    Forecast Results for the Year 2020:
              PRCP        TAVG        TMAX       TMIN
    0    11.327319   64.122055   70.571777  51.297550
    1    10.587886   43.023342   46.858006  33.289497
    2    10.553814   77.613403   84.169029  51.382168
    3    10.585902  103.433693  107.928841  73.283966
    4    10.412631   89.739044   95.140823  63.107113
    ..         ...         ...         ...        ...
    360  10.091131   68.870224   77.718628  56.535130
    361   9.012994   66.280487   73.534218  40.814228
    362  12.526095   79.747169   83.029556  59.272137
    363  15.670558   70.737312   72.355553  41.114422
    364  14.806677   75.998718   73.894165  40.316448
    
    [365 rows x 4 columns]
     mean avarage for Forecast Data 2020:
    PRCP    11.604603
    TAVG    74.189529
    TMAX    79.513847
    TMIN    53.745804
    dtype: float32
    


```python

```
