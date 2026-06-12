========== NUMPY NOTES ===============
        

1. What is NumPy?
   
NumPy (Numerical Python) is a Python library used for numerical and mathematical computations. It provides a powerful N-dimensional array (ndarray) that is faster and more memory-efficient than Python lists.

Import:
import numpy as np

-----------------------------------

2. NumPy Array
A NumPy array is a collection of elements of the same data type stored in contiguous memory locations.

Syntax:
np.array(data)

-----------------------------------

3. 0-D Array (Scalar)
• Contains only one element.
• Has no dimensions.

Example:
a = np.array(10)

ndim = 0
shape = ()

-----------------------------------

4. 1-D Array
• Contains a single row of elements.
• Similar to a Python list.

Example:
a = np.array([10,20,30,40])

ndim = 1
shape = (4,)

-----------------------------------

5. 2-D Array
• Contains rows and columns.
• Similar to a matrix.

Example:
a = np.array([[1,2,3],
              [4,5,6]])

ndim = 2
shape = (2,3)

-----------------------------------

6. 3-D Array
• Collection of 2-D arrays.
• Has depth, rows, and columns.

Example:
a = np.array([
[[1,2],[3,4]],
[[5,6],[7,8]]
])

ndim = 3
shape = (2,2,2)

-----------------------------------

7. 4-D Array
• Collection of 3-D arrays.
• Used in advanced applications like AI and image processing.

ndim = 4

-----------------------------------

8. Important NumPy Attributes

A) ndim
Returns the number of dimensions.

Syntax:
array.ndim

B) shape
Returns the size of each dimension.

Syntax:
array.shape

Examples:
0D -> ()
1D -> (5,)
2D -> (3,4)
3D -> (2,3,4)

C) size
Returns the total number of elements.

Syntax:
array.size

D) dtype
Returns the data type of array elements.

Syntax:
array.dtype

-----------------------------------

9. Python List vs NumPy Array

Python List:
• Slower
• More memory
• Different data types allowed

NumPy Array:
• Faster
• Less memory
• Efficient mathematical operations
• Usually same data type

-----------------------------------

10. Advantages of NumPy

• Fast computation
• Less memory usage
• Supports multidimensional arrays
• Easy mathematical operations
• Useful for Data Science, AI, ML, and Data Analysis

-----------------------------------

Important Interview Questions

Q1. What is NumPy?
Ans: NumPy is a Python library for numerical computing that provides support for multidimensional arrays and mathematical operations.

Q2. What is ndarray?
Ans: ndarray is the main data structure of NumPy used to store homogeneous data efficiently.

Q3. What does ndim do?
Ans: It returns the number of dimensions of an array.

Q4. What does shape return?
Ans: It returns the size of each dimension.

Q5. What does size return?
Ans: It returns the total number of elements in an array.

Q6. Difference between 1D and 2D arrays?
Ans:
1D -> Single row of elements.
2D -> Rows and columns (Matrix).

=========== END OF NOTES ==============

