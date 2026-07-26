# Week 4 — Data Analysis with NumPy & Pandas 📊

> *This is where Python gets powerful. We start working with real data.*

---

## 🎯 Learning Objectives
- Use NumPy for numerical computing
- Load, explore, and clean datasets with Pandas
- Filter, sort, group, and aggregate data
- Handle missing values like a professional

---

## 📂 Contents

| File | Description |
|------|-------------|
| `01_NumPy_Basics.ipynb` | Arrays, operations, broadcasting, indexing |
| `02_Pandas_Intro.ipynb` | Series, DataFrames, loading CSV/Excel |
| `03_Data_Exploration.ipynb` | .info(), .describe(), .head(), .shape |
| `04_Data_Cleaning.ipynb` | Missing values, duplicates, data types |
| `05_Data_Manipulation.ipynb` | Filtering, sorting, groupby, merging |
| `Week4_Exercises.ipynb` | Practice problems |
| `📁 Project/` | Week 4 project brief and starter notebook |
| `📁 datasets/` | Sample datasets for exercises |

---

## 📖 Key Concepts

### NumPy
```python
import numpy as np

arr = np.array([1, 2, 3, 4, 5])
print(arr.mean())    # 3.0
print(arr.std())     # 1.41
print(arr * 2)       # [2, 4, 6, 8, 10]
```

### Pandas — Loading & Exploring Data
```python
import pandas as pd

df = pd.read_csv("students.csv")
print(df.head())          # first 5 rows
print(df.shape)           # (rows, columns)
print(df.describe())      # statistics summary
print(df.isnull().sum())  # count missing values
```

### Data Cleaning
```python
# Drop missing values
df.dropna(inplace=True)

# Fill missing values
df['score'].fillna(df['score'].mean(), inplace=True)

# Remove duplicates
df.drop_duplicates(inplace=True)
```

### GroupBy & Aggregation
```python
# Average score by department
df.groupby('department')['score'].mean()

# Count students per city
df['city'].value_counts()
```

---

## 🚀 Week 4 Project
**📁 See `Project/` folder**

**Project: Student Performance Analysis**
- Dataset: Student exam scores CSV
- Tasks: Load data, clean it, explore patterns, answer business questions
- Deliverable: A completed Jupyter notebook with your analysis and conclusions

---

## 📝 Assignment
Complete `Week4_Exercises.ipynb` AND the project in `Project/`.
