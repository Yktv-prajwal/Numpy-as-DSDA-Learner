
## Lecture 2 NOTES


What is NumPy?
--------------
NumPy (Numerical Python) is a Python library used for:
• Working with arrays
• Mathematical calculations
• Scientific computing
• Data Analysis
• Machine Learning

Import NumPy:
import numpy as np

--------------------------------------------------

1. ARRAY
---------

An array is a collection of similar data stored in a single variable.

Example:
data = np.array([12,13,14,15,16,17])

Output:
[12 13 14 15 16 17]

--------------------------------------------------

2. INDEXING
------------

Indexing is used to access a single element from an array.

Positive Indexing:

Array : [12 13 14 15 16 17]
Index :  0  1  2  3  4  5

Examples:
data[0] = 12
data[2] = 14

Negative Indexing:

Array : [12 13 14 15 16 17]
Index : -6 -5 -4 -3 -2 -1

Examples:
data[-1] = 17
data[-2] = 16

--------------------------------------------------

3. SLICING
-----------

Slicing is used to access multiple elements.

Syntax:
array[start:end]

Note:
• Start index is included.
• End index is excluded.

Examples:

data[1:4]
Output:
[13 14 15]

data[:4]
Output:
[12 13 14 15]

data[2:]
Output:
[14 15 16 17]

data[:]
Output:
[12 13 14 15 16 17]

--------------------------------------------------

4. 2D ARRAY
------------

A 2D array consists of rows and columns.

Example:

data_2d = np.array([
    [21,22,23],
    [24,25,26],
    [27,28,29]
])

Representation:

[
 [21 22 23]
 [24 25 26]
 [27 28 29]
]

Rows = 3
Columns = 3

--------------------------------------------------

5. ndim
---------

ndim stands for Number of Dimensions.

Examples:

1D Array:
[1,2,3]
ndim = 1

2D Array:
[[1,2],
 [3,4]]
ndim = 2

3D Array:
[[[1,2],[3,4]]]
ndim = 3

Syntax:
array.ndim

--------------------------------------------------

6. shape
----------

shape returns the size of each dimension.

Example:

data_2d.shape

Output:
(3,3)

Meaning:
3 Rows
3 Columns

Syntax:
array.shape

--------------------------------------------------

7. ACCESSING ELEMENTS IN 2D ARRAY
----------------------------------

Syntax:
array[row,column]

Example:

data_2d[1,1]

Output:
25

Explanation:
Row 1 = [24 25 26]
Column 1 = 25

Example:

data_2d[0,1]

Output:
22

--------------------------------------------------

8. ACCESSING ROWS
------------------

First Row:

data_2d[0]

Output:
[21 22 23]

Second Row:

data_2d[1]

Output:
[24 25 26]

--------------------------------------------------

9. ACCESSING COLUMNS
---------------------

Syntax:
array[:,column]

Example:

data_2d[:,1]

Output:
[22 25 28]

Explanation:
: means all rows
1 means second column

--------------------------------------------------

10. 3D ARRAY
-------------

A 3D array is a collection of multiple 2D arrays.

Example:

arr_3d = np.array([
    [[1,2],[3,4]],
    [[5,6],[7,8]]
])

Representation:

[
 [
  [1 2]
  [3 4]
 ]

 [
  [5 6]
  [7 8]
 ]
]

Shape:
(2,2,2)

Meaning:
2 Blocks
2 Rows
2 Columns

--------------------------------------------------

11. ELLIPSIS (...)
------------------

Ellipsis (...) is a shortcut used to select all remaining dimensions.

Example:

arr_3d[...,0]

Output:

[
 [1 3]
 [5 7]
]

Example:

arr_3d[...,1]

Output:

[
 [2 4]
 [6 8]
]

--------------------------------------------------

12. ACCESSING SINGLE ELEMENT IN 3D ARRAY
-----------------------------------------

Syntax:
array[block][row,column]

Example:

arr_3d[1][0,1]

Output:
6

Explanation:

Block 1:

[
 [5 6]
 [7 8]
]

Row 0, Column 1 = 6

--------------------------------------------------

13. ACCESSING ROWS IN 3D ARRAY
-------------------------------

Example:

arr_3d[0][1,:]

Output:
[3 4]

Example:

arr_3d[1][1,:]

Output:
[7 8]

':' means select all columns.

--------------------------------------------------

14. RESHAPE()
--------------

reshape() changes the shape of an array without changing the data.

Syntax:

array.reshape(rows,columns)

Example:

data = np.array([11,12,13,14,15,16])

data.reshape(2,3)

Output:

[
 [11 12 13]
 [14 15 16]
]

Important Rule:

rows × columns = total elements

Example:

2 × 3 = 6
3 × 2 = 6
1 × 6 = 6

All are valid because total elements remain 6.

--------------------------------------------------

QUICK REVISION
--------------

Indexing:
arr[0]
arr[-1]

Slicing:
arr[1:4]
arr[:4]
arr[2:]
arr[:]

2D Access:
arr[row,column]

Column Access:
arr[:,1]

Array Information:
arr.ndim
arr.shape

3D Access:
arr_3d[1][0,1]
arr_3d[...,0]
arr_3d[...,1]

Reshape:
arr.reshape(rows,columns)

Remember:
Indexing → Single Value
Slicing → Multiple Values
ndim → Number of Dimensions
shape → Size of Dimensions
reshape() → Changes Structure
