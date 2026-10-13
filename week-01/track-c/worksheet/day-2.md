# Track C — Day 2 Worksheet — pandas

**Name:** Arslan Ahmad **GitHub handle:** https://github.com/arslaanahmad2005-dotcom
**Track:** Track C (ML Fundamentals)  **Day:** 2  **Date:** Tuesday 13 Oct 2026

**Video:** [pandas — Complete Data Science Course](https://youtu.be/QUaSmqBeR9w) ·
**Repo:** [AkarshVyas/Pandas-Youtube](https://github.com/AkarshVyas/Pandas-Youtube)

> Fill in the gaps. Run every snippet and paste the **real** output.

---

## Question 1 — Build a DataFrame

Create a DataFrame from the data below, then print its `head()`, `info()`, and `shape`.

| name | city | marks |
|---|---|---|
| Asha | Delhi | 78 |
| Ravi | Mumbai | 85 |
| Neha | Pune | 91 |

**Your code:**

```python
import pandas as pd

data = {
    "name": ["Asha", "Ravi", "Neha"],
    "city": ["Delhi", "Mumbai", "Pune"],
    "marks": [78, 85, 91]
}

df = pd.DataFrame(data)

print(df.head())
print(df.info())
print(df.shape)


```

**Output:**

```
   name    city  marks
0  Asha   Delhi     78
1  Ravi  Mumbai     85
2  Neha    Pune     91

<class 'pandas.core.frame.DataFrame'>
RangeIndex: 3 entries, 0 to 2
Data columns (total 3 columns):
 #   Column  Non-Null Count  Dtype
---  ------  --------------  -----
 0   name    3 non-null      object
 1   city    3 non-null      object
 2   marks   3 non-null      int64
dtypes: int64(1), object(2)
memory usage: 204.0+ bytes
None
(3, 3)
```

---

## Question 2 — Missing data and group-by

Load a small CSV of your choice (or build one) that has **at least one missing value**. Show the count
of missing values per column, fill or drop them, then group by a category column and print the average
of a numeric column.

**Your code:**

```python
# write your program here
import pandas as pd
import numpy as np

data = {
    "city": ["Delhi", "Mumbai", "Delhi", "Mumbai", "Pune"],
    "marks": [80, 75, np.nan, 90, 85]
}

df = pd.DataFrame(data)

print("Missing values:")
print(df.isnull().sum())

df["marks"] = df["marks"].fillna(df["marks"].mean())

print("\nData after filling missing values:")
print(df)

print("\nAverage marks by city:")
print(df.groupby("city")["marks"].mean())


```

**Output:**

```
Missing values:
city     0
marks    1
dtype: int64

Data after filling missing values:
     city  marks
0   Delhi   80.0
1  Mumbai   75.0
2   Delhi   82.5
3  Mumbai   90.0
4    Pune   85.0

Average marks by city:
city
Delhi     81.25
Mumbai    82.50
Pune      85.00
Name: marks, dtype: float64
```

**Which did you choose — fill or drop — and why?**
I chose to fill the missing value with the mean because it preserves all rows and avoids losing useful data.

---

## Question 3 — Case study: the video's capstone

Complete the **Data Capstone Project** from the video (`1:56:19`),
then answer: which pandas operations did the project rely on most, and what would you do differently on
your own dataset?

**Operations used most:**
The project relied on read_csv(), head(), info(), describe(), filtering, sorting, groupby(), and aggregation to clean, explore, and analyze data.


**What I would do differently:**
I would check for missing values and duplicate records first, clean inconsistent data, use meaningful column names, and create visualizations to understand trends more clearly.
