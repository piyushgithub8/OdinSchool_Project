```python
import numpy as np
a=np.array([[1,2,3],[4,5,6],[7,8,9]])
a
```




    array([[1, 2, 3],
           [4, 5, 6],
           [7, 8, 9]])




```python
a.ndim
```




    2




```python
b=np.full((3,3),7)
b
```




    array([[7, 7, 7],
           [7, 7, 7],
           [7, 7, 7]])




```python
c=np.linspace(10,20,30)
c
```




    array([10.        , 10.34482759, 10.68965517, 11.03448276, 11.37931034,
           11.72413793, 12.06896552, 12.4137931 , 12.75862069, 13.10344828,
           13.44827586, 13.79310345, 14.13793103, 14.48275862, 14.82758621,
           15.17241379, 15.51724138, 15.86206897, 16.20689655, 16.55172414,
           16.89655172, 17.24137931, 17.5862069 , 17.93103448, 18.27586207,
           18.62068966, 18.96551724, 19.31034483, 19.65517241, 20.        ])




```python
d=np.random.random((2,2))
d
```




    array([[0.74759034, 0.7287583 ],
           [0.18623019, 0.43737525]])




```python
e=np.array((1,2,3,4))
f=np.array((5,6,7,8))
np.concatenate((e,f),axis=0)
```




    array([1, 2, 3, 4, 5, 6, 7, 8])




```python

```


```python

```


```python
np.zeros(10)
```




    array([0., 0., 0., 0., 0., 0., 0., 0., 0., 0.])




```python
np.ones(10)
```




    array([1., 1., 1., 1., 1., 1., 1., 1., 1., 1.])




```python
np.full(10,5)
```




    array([5, 5, 5, 5, 5, 5, 5, 5, 5, 5])




```python
(np.ones(10))*5
```




    array([5., 5., 5., 5., 5., 5., 5., 5., 5., 5.])




```python
np.arange(10,31)
```




    array([10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26,
           27, 28, 29, 30])




```python
np.arange(10,52,2)
```




    array([10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42,
           44, 46, 48, 50])




```python
q=np.arange(0,9)
```


```python
q.reshape(3,3)
```




    array([[0, 1, 2],
           [3, 4, 5],
           [6, 7, 8]])




```python
np.eye(3)
```




    array([[1., 0., 0.],
           [0., 1., 0.],
           [0., 0., 1.]])




```python
np.random.random(1)
```




    array([0.31038408])




```python
np.random.randn(20)
```




    array([-0.10730838, -0.74122407,  1.66587685,  0.23991238, -2.02312963,
           -0.49032152,  0.99334408,  1.37336643, -0.83683828,  0.94957036,
           -0.76460067,  1.95213115,  0.75803596, -0.42575472,  0.1070206 ,
           -0.86235375,  0.91599405, -2.30605336, -1.46239319,  0.36019103])




```python
w=np.linspace(0,1,20)
w
```




    array([0.        , 0.05263158, 0.10526316, 0.15789474, 0.21052632,
           0.26315789, 0.31578947, 0.36842105, 0.42105263, 0.47368421,
           0.52631579, 0.57894737, 0.63157895, 0.68421053, 0.73684211,
           0.78947368, 0.84210526, 0.89473684, 0.94736842, 1.        ])




```python
w.ndim
```




    1




```python
np.matrix(np.linspace(0.01,1,100))
```




    matrix([[0.01, 0.02, 0.03, 0.04, 0.05, 0.06, 0.07, 0.08, 0.09, 0.1 ,
             0.11, 0.12, 0.13, 0.14, 0.15, 0.16, 0.17, 0.18, 0.19, 0.2 ,
             0.21, 0.22, 0.23, 0.24, 0.25, 0.26, 0.27, 0.28, 0.29, 0.3 ,
             0.31, 0.32, 0.33, 0.34, 0.35, 0.36, 0.37, 0.38, 0.39, 0.4 ,
             0.41, 0.42, 0.43, 0.44, 0.45, 0.46, 0.47, 0.48, 0.49, 0.5 ,
             0.51, 0.52, 0.53, 0.54, 0.55, 0.56, 0.57, 0.58, 0.59, 0.6 ,
             0.61, 0.62, 0.63, 0.64, 0.65, 0.66, 0.67, 0.68, 0.69, 0.7 ,
             0.71, 0.72, 0.73, 0.74, 0.75, 0.76, 0.77, 0.78, 0.79, 0.8 ,
             0.81, 0.82, 0.83, 0.84, 0.85, 0.86, 0.87, 0.88, 0.89, 0.9 ,
             0.91, 0.92, 0.93, 0.94, 0.95, 0.96, 0.97, 0.98, 0.99, 1.  ]])




```python

np.arange(1,101).reshape(10,10) / 100

```




    array([[0.01, 0.02, 0.03, 0.04, 0.05, 0.06, 0.07, 0.08, 0.09, 0.1 ],
           [0.11, 0.12, 0.13, 0.14, 0.15, 0.16, 0.17, 0.18, 0.19, 0.2 ],
           [0.21, 0.22, 0.23, 0.24, 0.25, 0.26, 0.27, 0.28, 0.29, 0.3 ],
           [0.31, 0.32, 0.33, 0.34, 0.35, 0.36, 0.37, 0.38, 0.39, 0.4 ],
           [0.41, 0.42, 0.43, 0.44, 0.45, 0.46, 0.47, 0.48, 0.49, 0.5 ],
           [0.51, 0.52, 0.53, 0.54, 0.55, 0.56, 0.57, 0.58, 0.59, 0.6 ],
           [0.61, 0.62, 0.63, 0.64, 0.65, 0.66, 0.67, 0.68, 0.69, 0.7 ],
           [0.71, 0.72, 0.73, 0.74, 0.75, 0.76, 0.77, 0.78, 0.79, 0.8 ],
           [0.81, 0.82, 0.83, 0.84, 0.85, 0.86, 0.87, 0.88, 0.89, 0.9 ],
           [0.91, 0.92, 0.93, 0.94, 0.95, 0.96, 0.97, 0.98, 0.99, 1.  ]])




```python
e=np.arange(1,26).reshape(5,5)
e
```




    array([[ 1,  2,  3,  4,  5],
           [ 6,  7,  8,  9, 10],
           [11, 12, 13, 14, 15],
           [16, 17, 18, 19, 20],
           [21, 22, 23, 24, 25]])




```python

```




    array([[ 1,  2,  3,  4,  5],
           [ 6,  7,  8,  9, 10],
           [11, 12, 13, 14, 15],
           [16, 17, 18, 19, 20],
           [21, 22, 23, 24, 25]])




```python
e[2:,1:]
```




    array([[12, 13, 14, 15],
           [17, 18, 19, 20],
           [22, 23, 24, 25]])




```python

```


```python

```


```python

```


```python
e[:2,1:2]
```




    array([[2],
           [7]])




```python
e
```




    array([[ 1,  2,  3,  4,  5],
           [ 6,  7,  8,  9, 10],
           [11, 12, 13, 14, 15],
           [16, 17, 18, 19, 20],
           [21, 22, 23, 24, 25]])




```python
np.sum(e, axis=0)
```




    array([55, 60, 65, 70, 75])




```python
np.sum(e, axis=1)
```




    array([ 15,  40,  65,  90, 115])




```python
car["am"]=1
car
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
      <th>Unnamed: 0</th>
      <th>mpg</th>
      <th>cyl</th>
      <th>disp</th>
      <th>hp</th>
      <th>drat</th>
      <th>wt</th>
      <th>qsec</th>
      <th>vs</th>
      <th>am</th>
      <th>gear</th>
      <th>carb</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Mazda RX4</td>
      <td>21.0</td>
      <td>6</td>
      <td>160.0</td>
      <td>110</td>
      <td>3.90</td>
      <td>2.620</td>
      <td>16.46</td>
      <td>0</td>
      <td>1</td>
      <td>4</td>
      <td>4</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Mazda RX4 Wag</td>
      <td>21.0</td>
      <td>6</td>
      <td>160.0</td>
      <td>110</td>
      <td>3.90</td>
      <td>2.875</td>
      <td>17.02</td>
      <td>0</td>
      <td>1</td>
      <td>4</td>
      <td>4</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Datsun 710</td>
      <td>22.8</td>
      <td>4</td>
      <td>108.0</td>
      <td>93</td>
      <td>3.85</td>
      <td>2.320</td>
      <td>18.61</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
      <td>1</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Hornet 4 Drive</td>
      <td>21.4</td>
      <td>6</td>
      <td>258.0</td>
      <td>110</td>
      <td>3.08</td>
      <td>3.215</td>
      <td>19.44</td>
      <td>1</td>
      <td>1</td>
      <td>3</td>
      <td>1</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Hornet Sportabout</td>
      <td>18.7</td>
      <td>8</td>
      <td>360.0</td>
      <td>175</td>
      <td>3.15</td>
      <td>3.440</td>
      <td>17.02</td>
      <td>0</td>
      <td>1</td>
      <td>3</td>
      <td>2</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Valiant</td>
      <td>18.1</td>
      <td>6</td>
      <td>225.0</td>
      <td>105</td>
      <td>2.76</td>
      <td>3.460</td>
      <td>20.22</td>
      <td>1</td>
      <td>1</td>
      <td>3</td>
      <td>1</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Duster 360</td>
      <td>14.3</td>
      <td>8</td>
      <td>360.0</td>
      <td>245</td>
      <td>3.21</td>
      <td>3.570</td>
      <td>15.84</td>
      <td>0</td>
      <td>1</td>
      <td>3</td>
      <td>4</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Merc 240D</td>
      <td>24.4</td>
      <td>4</td>
      <td>146.7</td>
      <td>62</td>
      <td>3.69</td>
      <td>3.190</td>
      <td>20.00</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
      <td>2</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Merc 230</td>
      <td>22.8</td>
      <td>4</td>
      <td>140.8</td>
      <td>95</td>
      <td>3.92</td>
      <td>3.150</td>
      <td>22.90</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
      <td>2</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Merc 280</td>
      <td>19.2</td>
      <td>6</td>
      <td>167.6</td>
      <td>123</td>
      <td>3.92</td>
      <td>3.440</td>
      <td>18.30</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
      <td>4</td>
    </tr>
    <tr>
      <th>10</th>
      <td>Merc 280C</td>
      <td>17.8</td>
      <td>6</td>
      <td>167.6</td>
      <td>123</td>
      <td>3.92</td>
      <td>3.440</td>
      <td>18.90</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
      <td>4</td>
    </tr>
    <tr>
      <th>11</th>
      <td>Merc 450SE</td>
      <td>16.4</td>
      <td>8</td>
      <td>275.8</td>
      <td>180</td>
      <td>3.07</td>
      <td>4.070</td>
      <td>17.40</td>
      <td>0</td>
      <td>1</td>
      <td>3</td>
      <td>3</td>
    </tr>
    <tr>
      <th>12</th>
      <td>Merc 450SL</td>
      <td>17.3</td>
      <td>8</td>
      <td>275.8</td>
      <td>180</td>
      <td>3.07</td>
      <td>3.730</td>
      <td>17.60</td>
      <td>0</td>
      <td>1</td>
      <td>3</td>
      <td>3</td>
    </tr>
    <tr>
      <th>13</th>
      <td>Merc 450SLC</td>
      <td>15.2</td>
      <td>8</td>
      <td>275.8</td>
      <td>180</td>
      <td>3.07</td>
      <td>3.780</td>
      <td>18.00</td>
      <td>0</td>
      <td>1</td>
      <td>3</td>
      <td>3</td>
    </tr>
    <tr>
      <th>14</th>
      <td>Cadillac Fleetwood</td>
      <td>10.4</td>
      <td>8</td>
      <td>472.0</td>
      <td>205</td>
      <td>2.93</td>
      <td>5.250</td>
      <td>17.98</td>
      <td>0</td>
      <td>1</td>
      <td>3</td>
      <td>4</td>
    </tr>
    <tr>
      <th>15</th>
      <td>Lincoln Continental</td>
      <td>10.4</td>
      <td>8</td>
      <td>460.0</td>
      <td>215</td>
      <td>3.00</td>
      <td>5.424</td>
      <td>17.82</td>
      <td>0</td>
      <td>1</td>
      <td>3</td>
      <td>4</td>
    </tr>
    <tr>
      <th>16</th>
      <td>Chrysler Imperial</td>
      <td>14.7</td>
      <td>8</td>
      <td>440.0</td>
      <td>230</td>
      <td>3.23</td>
      <td>5.345</td>
      <td>17.42</td>
      <td>0</td>
      <td>1</td>
      <td>3</td>
      <td>4</td>
    </tr>
    <tr>
      <th>17</th>
      <td>Fiat 128</td>
      <td>32.4</td>
      <td>4</td>
      <td>78.7</td>
      <td>66</td>
      <td>4.08</td>
      <td>2.200</td>
      <td>19.47</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
      <td>1</td>
    </tr>
    <tr>
      <th>18</th>
      <td>Honda Civic</td>
      <td>30.4</td>
      <td>4</td>
      <td>75.7</td>
      <td>52</td>
      <td>4.93</td>
      <td>1.615</td>
      <td>18.52</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
      <td>2</td>
    </tr>
    <tr>
      <th>19</th>
      <td>Toyota Corolla</td>
      <td>33.9</td>
      <td>4</td>
      <td>71.1</td>
      <td>65</td>
      <td>4.22</td>
      <td>1.835</td>
      <td>19.90</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
      <td>1</td>
    </tr>
    <tr>
      <th>20</th>
      <td>Toyota Corona</td>
      <td>21.5</td>
      <td>4</td>
      <td>120.1</td>
      <td>97</td>
      <td>3.70</td>
      <td>2.465</td>
      <td>20.01</td>
      <td>1</td>
      <td>1</td>
      <td>3</td>
      <td>1</td>
    </tr>
    <tr>
      <th>21</th>
      <td>Dodge Challenger</td>
      <td>15.5</td>
      <td>8</td>
      <td>318.0</td>
      <td>150</td>
      <td>2.76</td>
      <td>3.520</td>
      <td>16.87</td>
      <td>0</td>
      <td>1</td>
      <td>3</td>
      <td>2</td>
    </tr>
    <tr>
      <th>22</th>
      <td>AMC Javelin</td>
      <td>15.2</td>
      <td>8</td>
      <td>304.0</td>
      <td>150</td>
      <td>3.15</td>
      <td>3.435</td>
      <td>17.30</td>
      <td>0</td>
      <td>1</td>
      <td>3</td>
      <td>2</td>
    </tr>
    <tr>
      <th>23</th>
      <td>Camaro Z28</td>
      <td>13.3</td>
      <td>8</td>
      <td>350.0</td>
      <td>245</td>
      <td>3.73</td>
      <td>3.840</td>
      <td>15.41</td>
      <td>0</td>
      <td>1</td>
      <td>3</td>
      <td>4</td>
    </tr>
    <tr>
      <th>24</th>
      <td>Pontiac Firebird</td>
      <td>19.2</td>
      <td>8</td>
      <td>400.0</td>
      <td>175</td>
      <td>3.08</td>
      <td>3.845</td>
      <td>17.05</td>
      <td>0</td>
      <td>1</td>
      <td>3</td>
      <td>2</td>
    </tr>
    <tr>
      <th>25</th>
      <td>Fiat X1-9</td>
      <td>27.3</td>
      <td>4</td>
      <td>79.0</td>
      <td>66</td>
      <td>4.08</td>
      <td>1.935</td>
      <td>18.90</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
      <td>1</td>
    </tr>
    <tr>
      <th>26</th>
      <td>Porsche 914-2</td>
      <td>26.0</td>
      <td>4</td>
      <td>120.3</td>
      <td>91</td>
      <td>4.43</td>
      <td>2.140</td>
      <td>16.70</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
      <td>2</td>
    </tr>
    <tr>
      <th>27</th>
      <td>Lotus Europa</td>
      <td>30.4</td>
      <td>4</td>
      <td>95.1</td>
      <td>113</td>
      <td>3.77</td>
      <td>1.513</td>
      <td>16.90</td>
      <td>1</td>
      <td>1</td>
      <td>5</td>
      <td>2</td>
    </tr>
    <tr>
      <th>28</th>
      <td>Ford Pantera L</td>
      <td>15.8</td>
      <td>8</td>
      <td>351.0</td>
      <td>264</td>
      <td>4.22</td>
      <td>3.170</td>
      <td>14.50</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
      <td>4</td>
    </tr>
    <tr>
      <th>29</th>
      <td>Ferrari Dino</td>
      <td>19.7</td>
      <td>6</td>
      <td>145.0</td>
      <td>175</td>
      <td>3.62</td>
      <td>2.770</td>
      <td>15.50</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
      <td>6</td>
    </tr>
    <tr>
      <th>30</th>
      <td>Maserati Bora</td>
      <td>15.0</td>
      <td>8</td>
      <td>301.0</td>
      <td>335</td>
      <td>3.54</td>
      <td>3.570</td>
      <td>14.60</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
      <td>8</td>
    </tr>
    <tr>
      <th>31</th>
      <td>Volvo 142E</td>
      <td>21.4</td>
      <td>4</td>
      <td>121.0</td>
      <td>109</td>
      <td>4.11</td>
      <td>2.780</td>
      <td>18.60</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
      <td>2</td>
    </tr>
  </tbody>
</table>
</div>




```python
car['cyl'].sort_values(ascending=False)

```




    16    8
    30    8
    4     8
    28    8
    6     8
    24    8
    23    8
    22    8
    21    8
    11    8
    12    8
    13    8
    14    8
    15    8
    1     6
    29    6
    0     6
    10    6
    9     6
    5     6
    3     6
    17    4
    18    4
    19    4
    20    4
    8     4
    7     4
    25    4
    26    4
    27    4
    2     4
    31    4
    Name: cyl, dtype: int64




```python
car[(car['cyl']>6) & (car['hp']>300)]

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
      <th>Unnamed: 0</th>
      <th>mpg</th>
      <th>cyl</th>
      <th>disp</th>
      <th>hp</th>
      <th>drat</th>
      <th>wt</th>
      <th>qsec</th>
      <th>vs</th>
      <th>am</th>
      <th>gear</th>
      <th>carb</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>30</th>
      <td>Maserati Bora</td>
      <td>15.0</td>
      <td>8</td>
      <td>301.0</td>
      <td>335</td>
      <td>3.54</td>
      <td>3.57</td>
      <td>14.6</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
      <td>8</td>
    </tr>
  </tbody>
</table>
</div>




```python
car[(car['cyl']>6) & (car['hp']>300)]

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
      <th>Unnamed: 0</th>
      <th>mpg</th>
      <th>cyl</th>
      <th>disp</th>
      <th>hp</th>
      <th>drat</th>
      <th>wt</th>
      <th>qsec</th>
      <th>vs</th>
      <th>am</th>
      <th>gear</th>
      <th>carb</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>30</th>
      <td>Maserati Bora</td>
      <td>15.0</td>
      <td>8</td>
      <td>301.0</td>
      <td>335</td>
      <td>3.54</td>
      <td>3.57</td>
      <td>14.6</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
      <td>8</td>
    </tr>
  </tbody>
</table>
</div>




```python

```


```python

```


```python

```


```python

```


```python

```


```python

```

### Pandas


```python

```


```python

```


```python
import pandas as pd
car=pd.read_csv("C:/Users/Nikhil/Downloads/mtcars.csv")
car
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
      <th>Unnamed: 0</th>
      <th>mpg</th>
      <th>cyl</th>
      <th>disp</th>
      <th>hp</th>
      <th>drat</th>
      <th>wt</th>
      <th>qsec</th>
      <th>vs</th>
      <th>am</th>
      <th>gear</th>
      <th>carb</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Mazda RX4</td>
      <td>21.0</td>
      <td>6</td>
      <td>160.0</td>
      <td>110</td>
      <td>3.90</td>
      <td>2.620</td>
      <td>16.46</td>
      <td>0</td>
      <td>1</td>
      <td>4</td>
      <td>4</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Mazda RX4 Wag</td>
      <td>21.0</td>
      <td>6</td>
      <td>160.0</td>
      <td>110</td>
      <td>3.90</td>
      <td>2.875</td>
      <td>17.02</td>
      <td>0</td>
      <td>1</td>
      <td>4</td>
      <td>4</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Datsun 710</td>
      <td>22.8</td>
      <td>4</td>
      <td>108.0</td>
      <td>93</td>
      <td>3.85</td>
      <td>2.320</td>
      <td>18.61</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
      <td>1</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Hornet 4 Drive</td>
      <td>21.4</td>
      <td>6</td>
      <td>258.0</td>
      <td>110</td>
      <td>3.08</td>
      <td>3.215</td>
      <td>19.44</td>
      <td>1</td>
      <td>0</td>
      <td>3</td>
      <td>1</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Hornet Sportabout</td>
      <td>18.7</td>
      <td>8</td>
      <td>360.0</td>
      <td>175</td>
      <td>3.15</td>
      <td>3.440</td>
      <td>17.02</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>2</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Valiant</td>
      <td>18.1</td>
      <td>6</td>
      <td>225.0</td>
      <td>105</td>
      <td>2.76</td>
      <td>3.460</td>
      <td>20.22</td>
      <td>1</td>
      <td>0</td>
      <td>3</td>
      <td>1</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Duster 360</td>
      <td>14.3</td>
      <td>8</td>
      <td>360.0</td>
      <td>245</td>
      <td>3.21</td>
      <td>3.570</td>
      <td>15.84</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>4</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Merc 240D</td>
      <td>24.4</td>
      <td>4</td>
      <td>146.7</td>
      <td>62</td>
      <td>3.69</td>
      <td>3.190</td>
      <td>20.00</td>
      <td>1</td>
      <td>0</td>
      <td>4</td>
      <td>2</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Merc 230</td>
      <td>22.8</td>
      <td>4</td>
      <td>140.8</td>
      <td>95</td>
      <td>3.92</td>
      <td>3.150</td>
      <td>22.90</td>
      <td>1</td>
      <td>0</td>
      <td>4</td>
      <td>2</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Merc 280</td>
      <td>19.2</td>
      <td>6</td>
      <td>167.6</td>
      <td>123</td>
      <td>3.92</td>
      <td>3.440</td>
      <td>18.30</td>
      <td>1</td>
      <td>0</td>
      <td>4</td>
      <td>4</td>
    </tr>
    <tr>
      <th>10</th>
      <td>Merc 280C</td>
      <td>17.8</td>
      <td>6</td>
      <td>167.6</td>
      <td>123</td>
      <td>3.92</td>
      <td>3.440</td>
      <td>18.90</td>
      <td>1</td>
      <td>0</td>
      <td>4</td>
      <td>4</td>
    </tr>
    <tr>
      <th>11</th>
      <td>Merc 450SE</td>
      <td>16.4</td>
      <td>8</td>
      <td>275.8</td>
      <td>180</td>
      <td>3.07</td>
      <td>4.070</td>
      <td>17.40</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>3</td>
    </tr>
    <tr>
      <th>12</th>
      <td>Merc 450SL</td>
      <td>17.3</td>
      <td>8</td>
      <td>275.8</td>
      <td>180</td>
      <td>3.07</td>
      <td>3.730</td>
      <td>17.60</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>3</td>
    </tr>
    <tr>
      <th>13</th>
      <td>Merc 450SLC</td>
      <td>15.2</td>
      <td>8</td>
      <td>275.8</td>
      <td>180</td>
      <td>3.07</td>
      <td>3.780</td>
      <td>18.00</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>3</td>
    </tr>
    <tr>
      <th>14</th>
      <td>Cadillac Fleetwood</td>
      <td>10.4</td>
      <td>8</td>
      <td>472.0</td>
      <td>205</td>
      <td>2.93</td>
      <td>5.250</td>
      <td>17.98</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>4</td>
    </tr>
    <tr>
      <th>15</th>
      <td>Lincoln Continental</td>
      <td>10.4</td>
      <td>8</td>
      <td>460.0</td>
      <td>215</td>
      <td>3.00</td>
      <td>5.424</td>
      <td>17.82</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>4</td>
    </tr>
    <tr>
      <th>16</th>
      <td>Chrysler Imperial</td>
      <td>14.7</td>
      <td>8</td>
      <td>440.0</td>
      <td>230</td>
      <td>3.23</td>
      <td>5.345</td>
      <td>17.42</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>4</td>
    </tr>
    <tr>
      <th>17</th>
      <td>Fiat 128</td>
      <td>32.4</td>
      <td>4</td>
      <td>78.7</td>
      <td>66</td>
      <td>4.08</td>
      <td>2.200</td>
      <td>19.47</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
      <td>1</td>
    </tr>
    <tr>
      <th>18</th>
      <td>Honda Civic</td>
      <td>30.4</td>
      <td>4</td>
      <td>75.7</td>
      <td>52</td>
      <td>4.93</td>
      <td>1.615</td>
      <td>18.52</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
      <td>2</td>
    </tr>
    <tr>
      <th>19</th>
      <td>Toyota Corolla</td>
      <td>33.9</td>
      <td>4</td>
      <td>71.1</td>
      <td>65</td>
      <td>4.22</td>
      <td>1.835</td>
      <td>19.90</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
      <td>1</td>
    </tr>
    <tr>
      <th>20</th>
      <td>Toyota Corona</td>
      <td>21.5</td>
      <td>4</td>
      <td>120.1</td>
      <td>97</td>
      <td>3.70</td>
      <td>2.465</td>
      <td>20.01</td>
      <td>1</td>
      <td>0</td>
      <td>3</td>
      <td>1</td>
    </tr>
    <tr>
      <th>21</th>
      <td>Dodge Challenger</td>
      <td>15.5</td>
      <td>8</td>
      <td>318.0</td>
      <td>150</td>
      <td>2.76</td>
      <td>3.520</td>
      <td>16.87</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>2</td>
    </tr>
    <tr>
      <th>22</th>
      <td>AMC Javelin</td>
      <td>15.2</td>
      <td>8</td>
      <td>304.0</td>
      <td>150</td>
      <td>3.15</td>
      <td>3.435</td>
      <td>17.30</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>2</td>
    </tr>
    <tr>
      <th>23</th>
      <td>Camaro Z28</td>
      <td>13.3</td>
      <td>8</td>
      <td>350.0</td>
      <td>245</td>
      <td>3.73</td>
      <td>3.840</td>
      <td>15.41</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>4</td>
    </tr>
    <tr>
      <th>24</th>
      <td>Pontiac Firebird</td>
      <td>19.2</td>
      <td>8</td>
      <td>400.0</td>
      <td>175</td>
      <td>3.08</td>
      <td>3.845</td>
      <td>17.05</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>2</td>
    </tr>
    <tr>
      <th>25</th>
      <td>Fiat X1-9</td>
      <td>27.3</td>
      <td>4</td>
      <td>79.0</td>
      <td>66</td>
      <td>4.08</td>
      <td>1.935</td>
      <td>18.90</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
      <td>1</td>
    </tr>
    <tr>
      <th>26</th>
      <td>Porsche 914-2</td>
      <td>26.0</td>
      <td>4</td>
      <td>120.3</td>
      <td>91</td>
      <td>4.43</td>
      <td>2.140</td>
      <td>16.70</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
      <td>2</td>
    </tr>
    <tr>
      <th>27</th>
      <td>Lotus Europa</td>
      <td>30.4</td>
      <td>4</td>
      <td>95.1</td>
      <td>113</td>
      <td>3.77</td>
      <td>1.513</td>
      <td>16.90</td>
      <td>1</td>
      <td>1</td>
      <td>5</td>
      <td>2</td>
    </tr>
    <tr>
      <th>28</th>
      <td>Ford Pantera L</td>
      <td>15.8</td>
      <td>8</td>
      <td>351.0</td>
      <td>264</td>
      <td>4.22</td>
      <td>3.170</td>
      <td>14.50</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
      <td>4</td>
    </tr>
    <tr>
      <th>29</th>
      <td>Ferrari Dino</td>
      <td>19.7</td>
      <td>6</td>
      <td>145.0</td>
      <td>175</td>
      <td>3.62</td>
      <td>2.770</td>
      <td>15.50</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
      <td>6</td>
    </tr>
    <tr>
      <th>30</th>
      <td>Maserati Bora</td>
      <td>15.0</td>
      <td>8</td>
      <td>301.0</td>
      <td>335</td>
      <td>3.54</td>
      <td>3.570</td>
      <td>14.60</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
      <td>8</td>
    </tr>
    <tr>
      <th>31</th>
      <td>Volvo 142E</td>
      <td>21.4</td>
      <td>4</td>
      <td>121.0</td>
      <td>109</td>
      <td>4.11</td>
      <td>2.780</td>
      <td>18.60</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
      <td>2</td>
    </tr>
  </tbody>
</table>
</div>




```python
car.head(5)
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
      <th>Unnamed: 0</th>
      <th>mpg</th>
      <th>cyl</th>
      <th>disp</th>
      <th>hp</th>
      <th>drat</th>
      <th>wt</th>
      <th>qsec</th>
      <th>vs</th>
      <th>am</th>
      <th>gear</th>
      <th>carb</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Mazda RX4</td>
      <td>21.0</td>
      <td>6</td>
      <td>160.0</td>
      <td>110</td>
      <td>3.90</td>
      <td>2.620</td>
      <td>16.46</td>
      <td>0</td>
      <td>1</td>
      <td>4</td>
      <td>4</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Mazda RX4 Wag</td>
      <td>21.0</td>
      <td>6</td>
      <td>160.0</td>
      <td>110</td>
      <td>3.90</td>
      <td>2.875</td>
      <td>17.02</td>
      <td>0</td>
      <td>1</td>
      <td>4</td>
      <td>4</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Datsun 710</td>
      <td>22.8</td>
      <td>4</td>
      <td>108.0</td>
      <td>93</td>
      <td>3.85</td>
      <td>2.320</td>
      <td>18.61</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
      <td>1</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Hornet 4 Drive</td>
      <td>21.4</td>
      <td>6</td>
      <td>258.0</td>
      <td>110</td>
      <td>3.08</td>
      <td>3.215</td>
      <td>19.44</td>
      <td>1</td>
      <td>0</td>
      <td>3</td>
      <td>1</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Hornet Sportabout</td>
      <td>18.7</td>
      <td>8</td>
      <td>360.0</td>
      <td>175</td>
      <td>3.15</td>
      <td>3.440</td>
      <td>17.02</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>2</td>
    </tr>
  </tbody>
</table>
</div>




```python
car.head(10)
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
      <th>Unnamed: 0</th>
      <th>mpg</th>
      <th>cyl</th>
      <th>disp</th>
      <th>hp</th>
      <th>drat</th>
      <th>wt</th>
      <th>qsec</th>
      <th>vs</th>
      <th>am</th>
      <th>gear</th>
      <th>carb</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Mazda RX4</td>
      <td>21.0</td>
      <td>6</td>
      <td>160.0</td>
      <td>110</td>
      <td>3.90</td>
      <td>2.620</td>
      <td>16.46</td>
      <td>0</td>
      <td>1</td>
      <td>4</td>
      <td>4</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Mazda RX4 Wag</td>
      <td>21.0</td>
      <td>6</td>
      <td>160.0</td>
      <td>110</td>
      <td>3.90</td>
      <td>2.875</td>
      <td>17.02</td>
      <td>0</td>
      <td>1</td>
      <td>4</td>
      <td>4</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Datsun 710</td>
      <td>22.8</td>
      <td>4</td>
      <td>108.0</td>
      <td>93</td>
      <td>3.85</td>
      <td>2.320</td>
      <td>18.61</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
      <td>1</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Hornet 4 Drive</td>
      <td>21.4</td>
      <td>6</td>
      <td>258.0</td>
      <td>110</td>
      <td>3.08</td>
      <td>3.215</td>
      <td>19.44</td>
      <td>1</td>
      <td>0</td>
      <td>3</td>
      <td>1</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Hornet Sportabout</td>
      <td>18.7</td>
      <td>8</td>
      <td>360.0</td>
      <td>175</td>
      <td>3.15</td>
      <td>3.440</td>
      <td>17.02</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>2</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Valiant</td>
      <td>18.1</td>
      <td>6</td>
      <td>225.0</td>
      <td>105</td>
      <td>2.76</td>
      <td>3.460</td>
      <td>20.22</td>
      <td>1</td>
      <td>0</td>
      <td>3</td>
      <td>1</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Duster 360</td>
      <td>14.3</td>
      <td>8</td>
      <td>360.0</td>
      <td>245</td>
      <td>3.21</td>
      <td>3.570</td>
      <td>15.84</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
      <td>4</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Merc 240D</td>
      <td>24.4</td>
      <td>4</td>
      <td>146.7</td>
      <td>62</td>
      <td>3.69</td>
      <td>3.190</td>
      <td>20.00</td>
      <td>1</td>
      <td>0</td>
      <td>4</td>
      <td>2</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Merc 230</td>
      <td>22.8</td>
      <td>4</td>
      <td>140.8</td>
      <td>95</td>
      <td>3.92</td>
      <td>3.150</td>
      <td>22.90</td>
      <td>1</td>
      <td>0</td>
      <td>4</td>
      <td>2</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Merc 280</td>
      <td>19.2</td>
      <td>6</td>
      <td>167.6</td>
      <td>123</td>
      <td>3.92</td>
      <td>3.440</td>
      <td>18.30</td>
      <td>1</td>
      <td>0</td>
      <td>4</td>
      <td>4</td>
    </tr>
  </tbody>
</table>
</div>




```python
car['mpg']
```




    0     21.0
    1     21.0
    2     22.8
    3     21.4
    4     18.7
    5     18.1
    6     14.3
    7     24.4
    8     22.8
    9     19.2
    10    17.8
    11    16.4
    12    17.3
    13    15.2
    14    10.4
    15    10.4
    16    14.7
    17    32.4
    18    30.4
    19    33.9
    20    21.5
    21    15.5
    22    15.2
    23    13.3
    24    19.2
    25    27.3
    26    26.0
    27    30.4
    28    15.8
    29    19.7
    30    15.0
    31    21.4
    Name: mpg, dtype: float64




```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python
car.iloc[0:1,1:8]
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
      <th>mpg</th>
      <th>cyl</th>
      <th>disp</th>
      <th>hp</th>
      <th>drat</th>
      <th>wt</th>
      <th>qsec</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>21.0</td>
      <td>6</td>
      <td>160.0</td>
      <td>110</td>
      <td>3.9</td>
      <td>2.62</td>
      <td>16.46</td>
    </tr>
  </tbody>
</table>
</div>




```python
car.loc[:,'mpg':'qsec']

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
      <th>mpg</th>
      <th>cyl</th>
      <th>disp</th>
      <th>hp</th>
      <th>drat</th>
      <th>wt</th>
      <th>qsec</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>21.0</td>
      <td>6</td>
      <td>160.0</td>
      <td>110</td>
      <td>3.90</td>
      <td>2.620</td>
      <td>16.46</td>
    </tr>
    <tr>
      <th>1</th>
      <td>21.0</td>
      <td>6</td>
      <td>160.0</td>
      <td>110</td>
      <td>3.90</td>
      <td>2.875</td>
      <td>17.02</td>
    </tr>
    <tr>
      <th>2</th>
      <td>22.8</td>
      <td>4</td>
      <td>108.0</td>
      <td>93</td>
      <td>3.85</td>
      <td>2.320</td>
      <td>18.61</td>
    </tr>
    <tr>
      <th>3</th>
      <td>21.4</td>
      <td>6</td>
      <td>258.0</td>
      <td>110</td>
      <td>3.08</td>
      <td>3.215</td>
      <td>19.44</td>
    </tr>
    <tr>
      <th>4</th>
      <td>18.7</td>
      <td>8</td>
      <td>360.0</td>
      <td>175</td>
      <td>3.15</td>
      <td>3.440</td>
      <td>17.02</td>
    </tr>
    <tr>
      <th>5</th>
      <td>18.1</td>
      <td>6</td>
      <td>225.0</td>
      <td>105</td>
      <td>2.76</td>
      <td>3.460</td>
      <td>20.22</td>
    </tr>
    <tr>
      <th>6</th>
      <td>14.3</td>
      <td>8</td>
      <td>360.0</td>
      <td>245</td>
      <td>3.21</td>
      <td>3.570</td>
      <td>15.84</td>
    </tr>
    <tr>
      <th>7</th>
      <td>24.4</td>
      <td>4</td>
      <td>146.7</td>
      <td>62</td>
      <td>3.69</td>
      <td>3.190</td>
      <td>20.00</td>
    </tr>
    <tr>
      <th>8</th>
      <td>22.8</td>
      <td>4</td>
      <td>140.8</td>
      <td>95</td>
      <td>3.92</td>
      <td>3.150</td>
      <td>22.90</td>
    </tr>
    <tr>
      <th>9</th>
      <td>19.2</td>
      <td>6</td>
      <td>167.6</td>
      <td>123</td>
      <td>3.92</td>
      <td>3.440</td>
      <td>18.30</td>
    </tr>
    <tr>
      <th>10</th>
      <td>17.8</td>
      <td>6</td>
      <td>167.6</td>
      <td>123</td>
      <td>3.92</td>
      <td>3.440</td>
      <td>18.90</td>
    </tr>
    <tr>
      <th>11</th>
      <td>16.4</td>
      <td>8</td>
      <td>275.8</td>
      <td>180</td>
      <td>3.07</td>
      <td>4.070</td>
      <td>17.40</td>
    </tr>
    <tr>
      <th>12</th>
      <td>17.3</td>
      <td>8</td>
      <td>275.8</td>
      <td>180</td>
      <td>3.07</td>
      <td>3.730</td>
      <td>17.60</td>
    </tr>
    <tr>
      <th>13</th>
      <td>15.2</td>
      <td>8</td>
      <td>275.8</td>
      <td>180</td>
      <td>3.07</td>
      <td>3.780</td>
      <td>18.00</td>
    </tr>
    <tr>
      <th>14</th>
      <td>10.4</td>
      <td>8</td>
      <td>472.0</td>
      <td>205</td>
      <td>2.93</td>
      <td>5.250</td>
      <td>17.98</td>
    </tr>
    <tr>
      <th>15</th>
      <td>10.4</td>
      <td>8</td>
      <td>460.0</td>
      <td>215</td>
      <td>3.00</td>
      <td>5.424</td>
      <td>17.82</td>
    </tr>
    <tr>
      <th>16</th>
      <td>14.7</td>
      <td>8</td>
      <td>440.0</td>
      <td>230</td>
      <td>3.23</td>
      <td>5.345</td>
      <td>17.42</td>
    </tr>
    <tr>
      <th>17</th>
      <td>32.4</td>
      <td>4</td>
      <td>78.7</td>
      <td>66</td>
      <td>4.08</td>
      <td>2.200</td>
      <td>19.47</td>
    </tr>
    <tr>
      <th>18</th>
      <td>30.4</td>
      <td>4</td>
      <td>75.7</td>
      <td>52</td>
      <td>4.93</td>
      <td>1.615</td>
      <td>18.52</td>
    </tr>
    <tr>
      <th>19</th>
      <td>33.9</td>
      <td>4</td>
      <td>71.1</td>
      <td>65</td>
      <td>4.22</td>
      <td>1.835</td>
      <td>19.90</td>
    </tr>
    <tr>
      <th>20</th>
      <td>21.5</td>
      <td>4</td>
      <td>120.1</td>
      <td>97</td>
      <td>3.70</td>
      <td>2.465</td>
      <td>20.01</td>
    </tr>
    <tr>
      <th>21</th>
      <td>15.5</td>
      <td>8</td>
      <td>318.0</td>
      <td>150</td>
      <td>2.76</td>
      <td>3.520</td>
      <td>16.87</td>
    </tr>
    <tr>
      <th>22</th>
      <td>15.2</td>
      <td>8</td>
      <td>304.0</td>
      <td>150</td>
      <td>3.15</td>
      <td>3.435</td>
      <td>17.30</td>
    </tr>
    <tr>
      <th>23</th>
      <td>13.3</td>
      <td>8</td>
      <td>350.0</td>
      <td>245</td>
      <td>3.73</td>
      <td>3.840</td>
      <td>15.41</td>
    </tr>
    <tr>
      <th>24</th>
      <td>19.2</td>
      <td>8</td>
      <td>400.0</td>
      <td>175</td>
      <td>3.08</td>
      <td>3.845</td>
      <td>17.05</td>
    </tr>
    <tr>
      <th>25</th>
      <td>27.3</td>
      <td>4</td>
      <td>79.0</td>
      <td>66</td>
      <td>4.08</td>
      <td>1.935</td>
      <td>18.90</td>
    </tr>
    <tr>
      <th>26</th>
      <td>26.0</td>
      <td>4</td>
      <td>120.3</td>
      <td>91</td>
      <td>4.43</td>
      <td>2.140</td>
      <td>16.70</td>
    </tr>
    <tr>
      <th>27</th>
      <td>30.4</td>
      <td>4</td>
      <td>95.1</td>
      <td>113</td>
      <td>3.77</td>
      <td>1.513</td>
      <td>16.90</td>
    </tr>
    <tr>
      <th>28</th>
      <td>15.8</td>
      <td>8</td>
      <td>351.0</td>
      <td>264</td>
      <td>4.22</td>
      <td>3.170</td>
      <td>14.50</td>
    </tr>
    <tr>
      <th>29</th>
      <td>19.7</td>
      <td>6</td>
      <td>145.0</td>
      <td>175</td>
      <td>3.62</td>
      <td>2.770</td>
      <td>15.50</td>
    </tr>
    <tr>
      <th>30</th>
      <td>15.0</td>
      <td>8</td>
      <td>301.0</td>
      <td>335</td>
      <td>3.54</td>
      <td>3.570</td>
      <td>14.60</td>
    </tr>
    <tr>
      <th>31</th>
      <td>21.4</td>
      <td>4</td>
      <td>121.0</td>
      <td>109</td>
      <td>4.11</td>
      <td>2.780</td>
      <td>18.60</td>
    </tr>
  </tbody>
</table>
</div>




```python

```


```python
car.tail(5)
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
      <th>Unnamed: 0</th>
      <th>mpg</th>
      <th>cyl</th>
      <th>disp</th>
      <th>hp</th>
      <th>drat</th>
      <th>wt</th>
      <th>qsec</th>
      <th>vs</th>
      <th>am</th>
      <th>gear</th>
      <th>carb</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>27</th>
      <td>Lotus Europa</td>
      <td>30.4</td>
      <td>4</td>
      <td>95.1</td>
      <td>113</td>
      <td>3.77</td>
      <td>1.513</td>
      <td>16.9</td>
      <td>1</td>
      <td>1</td>
      <td>5</td>
      <td>2</td>
    </tr>
    <tr>
      <th>28</th>
      <td>Ford Pantera L</td>
      <td>15.8</td>
      <td>8</td>
      <td>351.0</td>
      <td>264</td>
      <td>4.22</td>
      <td>3.170</td>
      <td>14.5</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
      <td>4</td>
    </tr>
    <tr>
      <th>29</th>
      <td>Ferrari Dino</td>
      <td>19.7</td>
      <td>6</td>
      <td>145.0</td>
      <td>175</td>
      <td>3.62</td>
      <td>2.770</td>
      <td>15.5</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
      <td>6</td>
    </tr>
    <tr>
      <th>30</th>
      <td>Maserati Bora</td>
      <td>15.0</td>
      <td>8</td>
      <td>301.0</td>
      <td>335</td>
      <td>3.54</td>
      <td>3.570</td>
      <td>14.6</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
      <td>8</td>
    </tr>
    <tr>
      <th>31</th>
      <td>Volvo 142E</td>
      <td>21.4</td>
      <td>4</td>
      <td>121.0</td>
      <td>109</td>
      <td>4.11</td>
      <td>2.780</td>
      <td>18.6</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
      <td>2</td>
    </tr>
  </tbody>
</table>
</div>




```python
car.drop(car['carb'],axis=1, inplace=True)
```


```python
car
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
      <th>Unnamed: 0</th>
      <th>mpg</th>
      <th>cyl</th>
      <th>disp</th>
      <th>hp</th>
      <th>drat</th>
      <th>wt</th>
      <th>qsec</th>
      <th>vs</th>
      <th>am</th>
      <th>gear</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Mazda RX4</td>
      <td>21.0</td>
      <td>6</td>
      <td>160.0</td>
      <td>110</td>
      <td>3.90</td>
      <td>2.620</td>
      <td>16.46</td>
      <td>0</td>
      <td>1</td>
      <td>4</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Mazda RX4 Wag</td>
      <td>21.0</td>
      <td>6</td>
      <td>160.0</td>
      <td>110</td>
      <td>3.90</td>
      <td>2.875</td>
      <td>17.02</td>
      <td>0</td>
      <td>1</td>
      <td>4</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Datsun 710</td>
      <td>22.8</td>
      <td>4</td>
      <td>108.0</td>
      <td>93</td>
      <td>3.85</td>
      <td>2.320</td>
      <td>18.61</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Hornet 4 Drive</td>
      <td>21.4</td>
      <td>6</td>
      <td>258.0</td>
      <td>110</td>
      <td>3.08</td>
      <td>3.215</td>
      <td>19.44</td>
      <td>1</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Hornet Sportabout</td>
      <td>18.7</td>
      <td>8</td>
      <td>360.0</td>
      <td>175</td>
      <td>3.15</td>
      <td>3.440</td>
      <td>17.02</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Valiant</td>
      <td>18.1</td>
      <td>6</td>
      <td>225.0</td>
      <td>105</td>
      <td>2.76</td>
      <td>3.460</td>
      <td>20.22</td>
      <td>1</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Duster 360</td>
      <td>14.3</td>
      <td>8</td>
      <td>360.0</td>
      <td>245</td>
      <td>3.21</td>
      <td>3.570</td>
      <td>15.84</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Merc 240D</td>
      <td>24.4</td>
      <td>4</td>
      <td>146.7</td>
      <td>62</td>
      <td>3.69</td>
      <td>3.190</td>
      <td>20.00</td>
      <td>1</td>
      <td>0</td>
      <td>4</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Merc 230</td>
      <td>22.8</td>
      <td>4</td>
      <td>140.8</td>
      <td>95</td>
      <td>3.92</td>
      <td>3.150</td>
      <td>22.90</td>
      <td>1</td>
      <td>0</td>
      <td>4</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Merc 280</td>
      <td>19.2</td>
      <td>6</td>
      <td>167.6</td>
      <td>123</td>
      <td>3.92</td>
      <td>3.440</td>
      <td>18.30</td>
      <td>1</td>
      <td>0</td>
      <td>4</td>
    </tr>
    <tr>
      <th>10</th>
      <td>Merc 280C</td>
      <td>17.8</td>
      <td>6</td>
      <td>167.6</td>
      <td>123</td>
      <td>3.92</td>
      <td>3.440</td>
      <td>18.90</td>
      <td>1</td>
      <td>0</td>
      <td>4</td>
    </tr>
    <tr>
      <th>11</th>
      <td>Merc 450SE</td>
      <td>16.4</td>
      <td>8</td>
      <td>275.8</td>
      <td>180</td>
      <td>3.07</td>
      <td>4.070</td>
      <td>17.40</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>12</th>
      <td>Merc 450SL</td>
      <td>17.3</td>
      <td>8</td>
      <td>275.8</td>
      <td>180</td>
      <td>3.07</td>
      <td>3.730</td>
      <td>17.60</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>13</th>
      <td>Merc 450SLC</td>
      <td>15.2</td>
      <td>8</td>
      <td>275.8</td>
      <td>180</td>
      <td>3.07</td>
      <td>3.780</td>
      <td>18.00</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>14</th>
      <td>Cadillac Fleetwood</td>
      <td>10.4</td>
      <td>8</td>
      <td>472.0</td>
      <td>205</td>
      <td>2.93</td>
      <td>5.250</td>
      <td>17.98</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>15</th>
      <td>Lincoln Continental</td>
      <td>10.4</td>
      <td>8</td>
      <td>460.0</td>
      <td>215</td>
      <td>3.00</td>
      <td>5.424</td>
      <td>17.82</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>16</th>
      <td>Chrysler Imperial</td>
      <td>14.7</td>
      <td>8</td>
      <td>440.0</td>
      <td>230</td>
      <td>3.23</td>
      <td>5.345</td>
      <td>17.42</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>17</th>
      <td>Fiat 128</td>
      <td>32.4</td>
      <td>4</td>
      <td>78.7</td>
      <td>66</td>
      <td>4.08</td>
      <td>2.200</td>
      <td>19.47</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
    </tr>
    <tr>
      <th>18</th>
      <td>Honda Civic</td>
      <td>30.4</td>
      <td>4</td>
      <td>75.7</td>
      <td>52</td>
      <td>4.93</td>
      <td>1.615</td>
      <td>18.52</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
    </tr>
    <tr>
      <th>19</th>
      <td>Toyota Corolla</td>
      <td>33.9</td>
      <td>4</td>
      <td>71.1</td>
      <td>65</td>
      <td>4.22</td>
      <td>1.835</td>
      <td>19.90</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
    </tr>
    <tr>
      <th>20</th>
      <td>Toyota Corona</td>
      <td>21.5</td>
      <td>4</td>
      <td>120.1</td>
      <td>97</td>
      <td>3.70</td>
      <td>2.465</td>
      <td>20.01</td>
      <td>1</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>21</th>
      <td>Dodge Challenger</td>
      <td>15.5</td>
      <td>8</td>
      <td>318.0</td>
      <td>150</td>
      <td>2.76</td>
      <td>3.520</td>
      <td>16.87</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>22</th>
      <td>AMC Javelin</td>
      <td>15.2</td>
      <td>8</td>
      <td>304.0</td>
      <td>150</td>
      <td>3.15</td>
      <td>3.435</td>
      <td>17.30</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>23</th>
      <td>Camaro Z28</td>
      <td>13.3</td>
      <td>8</td>
      <td>350.0</td>
      <td>245</td>
      <td>3.73</td>
      <td>3.840</td>
      <td>15.41</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>24</th>
      <td>Pontiac Firebird</td>
      <td>19.2</td>
      <td>8</td>
      <td>400.0</td>
      <td>175</td>
      <td>3.08</td>
      <td>3.845</td>
      <td>17.05</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>25</th>
      <td>Fiat X1-9</td>
      <td>27.3</td>
      <td>4</td>
      <td>79.0</td>
      <td>66</td>
      <td>4.08</td>
      <td>1.935</td>
      <td>18.90</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
    </tr>
    <tr>
      <th>26</th>
      <td>Porsche 914-2</td>
      <td>26.0</td>
      <td>4</td>
      <td>120.3</td>
      <td>91</td>
      <td>4.43</td>
      <td>2.140</td>
      <td>16.70</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
    </tr>
    <tr>
      <th>27</th>
      <td>Lotus Europa</td>
      <td>30.4</td>
      <td>4</td>
      <td>95.1</td>
      <td>113</td>
      <td>3.77</td>
      <td>1.513</td>
      <td>16.90</td>
      <td>1</td>
      <td>1</td>
      <td>5</td>
    </tr>
    <tr>
      <th>28</th>
      <td>Ford Pantera L</td>
      <td>15.8</td>
      <td>8</td>
      <td>351.0</td>
      <td>264</td>
      <td>4.22</td>
      <td>3.170</td>
      <td>14.50</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
    </tr>
    <tr>
      <th>29</th>
      <td>Ferrari Dino</td>
      <td>19.7</td>
      <td>6</td>
      <td>145.0</td>
      <td>175</td>
      <td>3.62</td>
      <td>2.770</td>
      <td>15.50</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
    </tr>
    <tr>
      <th>30</th>
      <td>Maserati Bora</td>
      <td>15.0</td>
      <td>8</td>
      <td>301.0</td>
      <td>335</td>
      <td>3.54</td>
      <td>3.570</td>
      <td>14.60</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
    </tr>
    <tr>
      <th>31</th>
      <td>Volvo 142E</td>
      <td>21.4</td>
      <td>4</td>
      <td>121.0</td>
      <td>109</td>
      <td>4.11</td>
      <td>2.780</td>
      <td>18.60</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
    </tr>
  </tbody>
</table>
</div>




```python

```


```python
car.isnull().sum()
```




    Unnamed: 0    0
    mpg           0
    cyl           0
    disp          0
    hp            0
    drat          0
    wt            0
    qsec          0
    vs            0
    am            0
    gear          0
    dtype: int64




```python
car.info()
```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 32 entries, 0 to 31
    Data columns (total 11 columns):
     #   Column      Non-Null Count  Dtype  
    ---  ------      --------------  -----  
     0   Unnamed: 0  32 non-null     object 
     1   mpg         32 non-null     float64
     2   cyl         32 non-null     int64  
     3   disp        32 non-null     float64
     4   hp          32 non-null     int64  
     5   drat        32 non-null     float64
     6   wt          32 non-null     float64
     7   qsec        32 non-null     float64
     8   vs          32 non-null     int64  
     9   am          32 non-null     int64  
     10  gear        32 non-null     int64  
    dtypes: float64(5), int64(5), object(1)
    memory usage: 2.7+ KB
    


```python
car.iloc[:,4]

```




    0     110
    1     110
    2      93
    3     110
    4     175
    5     105
    6     245
    7      62
    8      95
    9     123
    10    123
    11    180
    12    180
    13    180
    14    205
    15    215
    16    230
    17     66
    18     52
    19     65
    20     97
    21    150
    22    150
    23    245
    24    175
    25     66
    26     91
    27    113
    28    264
    29    175
    30    335
    31    109
    Name: hp, dtype: int64




```python
car.iloc[7:,4:]
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
      <th>hp</th>
      <th>drat</th>
      <th>wt</th>
      <th>qsec</th>
      <th>vs</th>
      <th>am</th>
      <th>gear</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>7</th>
      <td>62</td>
      <td>3.69</td>
      <td>3.190</td>
      <td>20.00</td>
      <td>1</td>
      <td>0</td>
      <td>4</td>
    </tr>
    <tr>
      <th>8</th>
      <td>95</td>
      <td>3.92</td>
      <td>3.150</td>
      <td>22.90</td>
      <td>1</td>
      <td>0</td>
      <td>4</td>
    </tr>
    <tr>
      <th>9</th>
      <td>123</td>
      <td>3.92</td>
      <td>3.440</td>
      <td>18.30</td>
      <td>1</td>
      <td>0</td>
      <td>4</td>
    </tr>
    <tr>
      <th>10</th>
      <td>123</td>
      <td>3.92</td>
      <td>3.440</td>
      <td>18.90</td>
      <td>1</td>
      <td>0</td>
      <td>4</td>
    </tr>
    <tr>
      <th>11</th>
      <td>180</td>
      <td>3.07</td>
      <td>4.070</td>
      <td>17.40</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>12</th>
      <td>180</td>
      <td>3.07</td>
      <td>3.730</td>
      <td>17.60</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>13</th>
      <td>180</td>
      <td>3.07</td>
      <td>3.780</td>
      <td>18.00</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>14</th>
      <td>205</td>
      <td>2.93</td>
      <td>5.250</td>
      <td>17.98</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>15</th>
      <td>215</td>
      <td>3.00</td>
      <td>5.424</td>
      <td>17.82</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>16</th>
      <td>230</td>
      <td>3.23</td>
      <td>5.345</td>
      <td>17.42</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>17</th>
      <td>66</td>
      <td>4.08</td>
      <td>2.200</td>
      <td>19.47</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
    </tr>
    <tr>
      <th>18</th>
      <td>52</td>
      <td>4.93</td>
      <td>1.615</td>
      <td>18.52</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
    </tr>
    <tr>
      <th>19</th>
      <td>65</td>
      <td>4.22</td>
      <td>1.835</td>
      <td>19.90</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
    </tr>
    <tr>
      <th>20</th>
      <td>97</td>
      <td>3.70</td>
      <td>2.465</td>
      <td>20.01</td>
      <td>1</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>21</th>
      <td>150</td>
      <td>2.76</td>
      <td>3.520</td>
      <td>16.87</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>22</th>
      <td>150</td>
      <td>3.15</td>
      <td>3.435</td>
      <td>17.30</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>23</th>
      <td>245</td>
      <td>3.73</td>
      <td>3.840</td>
      <td>15.41</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>24</th>
      <td>175</td>
      <td>3.08</td>
      <td>3.845</td>
      <td>17.05</td>
      <td>0</td>
      <td>0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>25</th>
      <td>66</td>
      <td>4.08</td>
      <td>1.935</td>
      <td>18.90</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
    </tr>
    <tr>
      <th>26</th>
      <td>91</td>
      <td>4.43</td>
      <td>2.140</td>
      <td>16.70</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
    </tr>
    <tr>
      <th>27</th>
      <td>113</td>
      <td>3.77</td>
      <td>1.513</td>
      <td>16.90</td>
      <td>1</td>
      <td>1</td>
      <td>5</td>
    </tr>
    <tr>
      <th>28</th>
      <td>264</td>
      <td>4.22</td>
      <td>3.170</td>
      <td>14.50</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
    </tr>
    <tr>
      <th>29</th>
      <td>175</td>
      <td>3.62</td>
      <td>2.770</td>
      <td>15.50</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
    </tr>
    <tr>
      <th>30</th>
      <td>335</td>
      <td>3.54</td>
      <td>3.570</td>
      <td>14.60</td>
      <td>0</td>
      <td>1</td>
      <td>5</td>
    </tr>
    <tr>
      <th>31</th>
      <td>109</td>
      <td>4.11</td>
      <td>2.780</td>
      <td>18.60</td>
      <td>1</td>
      <td>1</td>
      <td>4</td>
    </tr>
  </tbody>
</table>
</div>




```python

```


```python
df=(1,2,3,4,5,6,7,8,9,0)
a=pd.Series(df,index=['a','b','c','d','e','f','g','h','i','j'])
a
```




    a    1
    b    2
    c    3
    d    4
    e    5
    f    6
    g    7
    h    8
    i    9
    j    0
    dtype: int64




```python
dict={"A":["5"], "B":["9"]}
type(dict)
```




    dict




```python
df1_df=pd.DataFrame(dict)
df1_df
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
      <th>A</th>
      <th>B</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>5</td>
      <td>9</td>
    </tr>
  </tbody>
</table>
</div>




```python

```


```python

```
