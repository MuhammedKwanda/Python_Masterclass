# Week 5 — Data Visualization 📈

> *A picture is worth a thousand rows of data.*

---

## 🎯 Learning Objectives
- Create professional charts with Matplotlib
- Build statistical visualizations with Seaborn
- Choose the right chart for the right data
- Tell a story with your visualizations

---

## 📂 Contents

| File | Description |
|------|-------------|
| `01_Matplotlib_Basics.ipynb` | Line, bar, scatter, pie charts |
| `02_Matplotlib_Advanced.ipynb` | Subplots, styling, customization |
| `03_Seaborn_Basics.ipynb` | Distribution, categorical, relational plots |
| `04_Seaborn_Advanced.ipynb` | Heatmaps, pairplots, advanced styling |
| `05_Choosing_Right_Chart.ipynb` | When to use which visualization |
| `Week5_Exercises.ipynb` | Practice problems |
| `📁 Project/` | Week 5 project brief |

---

## 📖 Key Concepts

### Matplotlib
```python
import matplotlib.pyplot as plt

# Line chart
plt.plot([1,2,3,4], [10,20,15,30], color='blue', linewidth=2)
plt.title("Sales Over Time")
plt.xlabel("Month")
plt.ylabel("Sales")
plt.show()

# Bar chart
categories = ['Math', 'Science', 'English']
scores = [85, 92, 78]
plt.bar(categories, scores, color='steelblue')
plt.show()
```

### Seaborn
```python
import seaborn as sns

# Distribution plot
sns.histplot(df['score'], kde=True)

# Heatmap — great for correlations
sns.heatmap(df.corr(), annot=True, cmap='coolwarm')

# Boxplot — compare groups
sns.boxplot(x='gender', y='math_score', data=df)
```

---

## 🚀 Week 5 Project
**📁 See `Project/` folder**

**Project: Sales Dashboard Visualization**
- Create a complete visual analysis report with at least 6 different chart types
- Tell a data story: what happened, why it matters, what to do next

---

## 📝 Assignment
Complete `Week5_Exercises.ipynb` AND the project.
