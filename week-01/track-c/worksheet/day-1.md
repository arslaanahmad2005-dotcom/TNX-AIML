# Track C — Day 1 Worksheet — numpy

**Name:** Arslan Ahmad **GitHub handle:** https://github.com/arslaanahmad2005-dotcom
**Track:** Track C (ML Fundamentals)  **Day:** 1  **Date:** Monday 12 Oct 2026

**Video:** [numpy — Complete Data Science Course](https://youtu.be/Utgwk0r9Zq4) ·
**Capstone:** [`exersises.ipynb`](https://github.com/AkarshVyas/Numpy-Youtube/blob/main/exersises.ipynb)

> Fill in the gaps. Run every snippet and paste the **real** output.

---

## Question 1 — Create and inspect an array

Create a numpy array of the numbers 10, 20, 30, 40, 50. Print the array, its `shape`, its `dtype`, and
its mean.

**Your code:**

```python
import numpy as np

arr = np.array([10, 20, 30, 40, 50])

print(arr)
print("Shape:", arr.shape)
print("Data type:", arr.dtype)
print("Mean:", arr.mean())


```

**Output:**

```
_[10 20 30 40 50]
Shape: (5,)
Data type: int64
Mean: 30.0
```

**Why is a numpy array preferred over a Python list for numeric work?**
NumPy arrays are faster, use memory efficiently, and support mathematical operations on entire arrays.

---

## Question 2 — Indexing and slicing

Start with the 3×3 matrix below. Print: the element at row 1, column 2; the second row; the first
column; and every element greater than 3.

```python
m = np.array([[1, 2, 3],
              [4, 5, 6],
              [7, 8, 9]])
```

**Your code:**

```python
# write your program here
import numpy as np

m = np.array([[1, 2, 3],
              [4, 5, 6],
              [7, 8, 9]])

print("Row 1, column 2:", m[0, 1])
print("Second row:", m[1, :])
print("First column:", m[:, 0])
print("Elements greater than 3:", m[m > 3])

```

**Output:**

```
Row 1, column 2: 2
Second row: [4 5 6]
First column: [1 4 7]
Elements greater than 3: [4 5 6 7 8 9]
```

---

## Question 3 — Case study: class marks

A class scored these marks:
`[72, 85, 90, 66, 78, 88, 95, 60, 74, 81]`.

Using numpy, compute the **mean, median, highest, lowest, and standard deviation**, then print how many
students scored above the mean.

**Your code:**

```python
# write your program here
import numpy as np

marks = np.array([72, 85, 90, 66, 78, 88, 95, 60, 74, 81])

print("Mean:", np.mean(marks))
print("Median:", np.median(marks))
print("Highest:", np.max(marks))
print("Lowest:", np.min(marks))
print("Standard deviation:", np.std(marks))
print("Students above mean:", np.sum(marks > np.mean(marks)))

```

**Output:**

```
Mean: 78.9
Median: 79.5
Highest: 95
Lowest: 60
Standard deviation: 10.501904589168577
Students above mean: 5
```

**How did you count the students above the mean in a single expression?**
Using np.sum(marks > np.mean(marks)), which counts the students whose marks are greater than the mean.
