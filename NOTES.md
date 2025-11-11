# NumPy Sorting – Quick Reference Guide

A clean and simple guide explaining how sorting works in NumPy, with examples for numbers, strings, booleans, 1D & 2D arrays, ascending/descending sorting, and axis-based sorting.

---

## 📘 What is Sorting?

Sorting means arranging elements in a specific order:
- Numeric or alphabetical  
- Ascending or descending  
- Frequently used in **data preprocessing**, **ranking**, **filtering**, and **ML pipelines**

---

## ✅ NumPy `sort()` Function

NumPy provides a built-in, efficient method:

### python
np.sort(array)
✔ Fast
✔ Works on all data types
✔ Very easy to use

### 🔹 Sorting Numbers (1D)
python
Copy code
import numpy as np

arr = np.array([3, 2, 0, 1])
print(np.sort(arr))
Output:

csharp
Copy code
[0 1 2 3]
### 🔹 Sorting Strings (1D)
python
Copy code
arr = np.array(['banana', 'cherry', 'apple'])
print(np.sort(arr))
Output:

css
Copy code
['apple', 'banana', 'cherry']
### 🔹 Sorting Booleans
python
Copy code
arr = np.array([True, False, True])
print(np.sort(arr))
Output:

graphql
Copy code
[False  True  True]
False (0) → True (1)

### 🔹 Sorting 2D Arrays (Each row sorted)
python
Copy code
arr = np.array([[3, 2, 4],
                [5, 0, 1]])
print(np.sort(arr))
### 🔹 Ascending & Descending Order
python
Copy code
a = np.array([110, 20, -30, 40])

# Ascending
print(np.sort(a))

# Descending
print(np.sort(a)[::-1])
### 🔹 Column-wise Sorting (axis=0)
python
Copy code
np.sort(a, axis=0)
Each column is sorted independently.

### 🔹 Row-wise Sorting (axis=1)
python
Copy code
np.sort(a, axis=1)
Each row is sorted independently.

### ✅ Summary
np.sort() is fast, clean, and powerful

Works on numbers, strings, booleans, and matrices

Very useful for ML, preprocessing, analytics, and data cleaning

