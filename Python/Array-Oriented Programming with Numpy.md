# 7.2 Creating arrays from existing data
The NumPy documentation recommends importing the **numpy module** as np so that you can acess its members with "np. ":

```python
import numpy as np 
```

numpy module provides various function for creating arrays. Here we use the array function, which receives as an argument as array or other collection of elements and returns a new array containing the arguments elements. lets pass a list:
```python
numbers = np.array([2,3,4,5,66])
```

The array function copies its arguments contents into the array. Lets look at the type of object that function array returns and display its contents:
```python
type(numbers)
# output numpy.ndarray
numbers
#array([ 2, 3, 4, 5, 66])
```

Note that the type is numpy.ndarray, but all arrays are output as "array". When output-ting an array NumPy separates each value form the next with a comma and a space and right-aligns all the values using the same field width. It determines the field width based on the value that occupies the largest number of character positions. In this case, the value 66 occupies the two character positions, so all the values are formatted in two-character fields. Thats why theres a leading space between the [ and 2 .

## Multidimensional Arguments
The array function copies its arguments dimensions. Lets create an array form a two-row-three-column list :

```python
np.array([[1,2,3],[4,5,6]])

# output: 
#        array([[1,2,3],
#               [4,5,6]])
# 
```

NumPy auto-formats arrays, based on their number of dimensions, aligning the columns within each row.
