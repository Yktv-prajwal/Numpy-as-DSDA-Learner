
# LECTURE 3 NOTES

# Import NumPy
import numpy as np

# Import Random Module
from numpy import random


# 1. randint()
# Generates random integers.
x = random.randint(100)
print(x)

# Random integer between 1 and 99
x = random.randint(1, 100)
print(x)

# 2D array of random integers
x = random.randint(100, size=(3,5))
print(x)


# 2. rand()
# Generates random float values between 0 and 1.

# Single float value
x = random.rand()
print(x)

# 1D float array
x = random.rand(5)
print(x)

# 2D float array
x = random.rand(3,5)
print(x)


# 3. choice()
# Selects random values from a given array.

# Single random value
x = random.choice([3,4,5,6,7,8,9,10])
print(x)

# Create 2D array using choice
x = random.choice([1,2,3,4,5,6,7,8,9], size=(3,3))
print(x)

# Random strings
colour = ["red","green","blue","lightgreen","pink"]
selected = random.choice(colour, size=3)
print(selected)


# 4. shuffle()
# Shuffles the original array.

arr = np.array([21,22,23,24,25])
np.random.shuffle(arr)
print(arr)


# 5. permutation()
# Returns a shuffled copy without changing original array.

arr = np.array([21,22,23,24,25])
new_arr = np.random.permutation(arr)
print(new_arr)


# 6. seed()
# Generates the same random values every time.

np.random.seed(42)
x = np.random.randint(1,100)
print(x)


# ==========================
# IMPORTANT FUNCTIONS
# ==========================

# random.randint(n)
# Random integer from 0 to n-1

# random.randint(a,b)
# Random integer from a to b-1

# random.randint(size=(r,c))
# Random integer array

# random.rand()
# Single float between 0 and 1

# random.rand(n)
# 1D float array

# random.rand(r,c)
# 2D float array

# random.choice()
# Random element from a list

# random.choice(size=(r,c))
# Random array from given values

# np.random.shuffle()
# Shuffles original array

# np.random.permutation()
# Returns shuffled copy

# np.random.seed()
# Fixes random output for reproducibility


# Viva Questions:
# 1. randint() -> Random integers.
# 2. rand() -> Random float values (0 to 1).
# 3. choice() -> Randomly selects elements.
# 4. shuffle() -> Shuffles original array.
# 5. permutation() -> Returns shuffled copy.
# 6. seed() -> Produces the same random sequence each run.
