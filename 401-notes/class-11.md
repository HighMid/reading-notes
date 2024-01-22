## Class 11 Notes

1. **What are the key features and benefits of Jupyter Lab, and how does it differ from Jupyter Notebook?**

    - Jupyter Lab is considered an upgrade to Jupyter Notebook by providing more of a comprehensive and powerful environment. Jupyter Lab features very flexible user interface over Jupyter Notebook and allows multiple notebooks to be opened in tabs similar to a browser.  It also integrates other components such as terminals, text editors, data file viewers etc. 

2. **What are the main functionalities provided by the NumPy library, and how can it be useful in Python programming, particularly for scientific computing and data manipulation tasks?**

    - NumPy is a library that has a vast amount of resources to help with mathematical functions, broadcasting capabilities and high-performance array operations. This is coupled with the large community support with extensive documentation, key features that help with data manipulation are:
        
        - Performance: Numpy provides an efficient way to store and manipulate arrays with performance in mind.
        - Data analysis: Usage of higher-level tools like Pandas
        - Machine Learning: Used in data preprocessing, transformation and manipulation in machine learning workflows.

3. **Explain the basic structure and properties of NumPy arrays, and provide examples of how to create, manipulate, and perform operations on them.**

    - NumPy arrays are n-dimensional, homogeneous arrays, which means that the arrays are fixed in size upon creation.

    > Elements are accessed by their index, the shape of the array is a tuple of integers determining the size of each dimension.

```
import numpy as np

# Creating from a Python list
a = np.array([1, 2, 3])

# Creating a zero-initialized array
b = np.zeros((3, 3))

# Creating an array with a specific range of numbers
c = np.arange(10)
```

```
# Reshaping an array
reshaped = a.reshape((3, 1))

# Basic arithmetic operations on arrays
sum_arrays = a + np.array([4, 5, 6])

# Applying a mathematical function
squared = np.square(a)

# Boolean indexing
filtered = a[a > 1]
```