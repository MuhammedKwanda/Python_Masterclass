# Week 6 — Machine Learning Basics 🤖

> *Teaching machines to learn from data.*

---

## 🎯 Learning Objectives
- Understand what Machine Learning is and how it works
- Know the difference between supervised and unsupervised learning
- Build your first regression and classification models
- Evaluate model performance properly

---

## 📂 Contents

| File | Description |
|------|-------------|
| `01_Intro_to_ML.ipynb` | What is ML, types, real-world applications |
| `02_ML_Workflow.ipynb` | Data → Features → Model → Evaluate → Deploy |
| `03_Linear_Regression.ipynb` | Predicting continuous values |
| `04_Logistic_Regression.ipynb` | Binary classification |
| `05_Model_Evaluation.ipynb` | Accuracy, precision, recall, F1, confusion matrix |
| `06_Train_Test_Split.ipynb` | Why we split data, overfitting vs underfitting |
| `Week6_Exercises.ipynb` | Practice problems |
| `📁 Project/` | Week 6 project brief |

---

## 📖 Key Concepts

### The ML Workflow
```
Raw Data → Clean Data → Feature Engineering → Train Model → Evaluate → Improve → Deploy
```

### Linear Regression
```python
from sklearn.linear_model import LinearRegression
from sklearn.model_selection import train_test_split
from sklearn.metrics import mean_squared_error

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

model = LinearRegression()
model.fit(X_train, y_train)

predictions = model.predict(X_test)
print(f"MSE: {mean_squared_error(y_test, predictions):.2f}")
```

### Classification & Evaluation
```python
from sklearn.metrics import classification_report, confusion_matrix

print(classification_report(y_test, predictions))
print(confusion_matrix(y_test, predictions))
```

---

## 🚀 Week 6 Project
**📁 See `Project/` folder**

**Project: House Price Prediction**
- Use regression to predict house prices from features
- Evaluate your model and explain the results

---

## 📝 Assignment
Complete `Week6_Exercises.ipynb` AND the project.
