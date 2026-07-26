# Week 7 — Machine Learning Advanced 🧠

> *Better models, smarter decisions.*

---

## 🎯 Learning Objectives
- Build and tune Random Forest and Decision Tree models
- Understand and handle class imbalance
- Build proper ML pipelines
- Apply feature engineering techniques
- Interpret model results

---

## 📂 Contents

| File | Description |
|------|-------------|
| `01_Decision_Trees.ipynb` | How trees work, visualization, pruning |
| `02_Random_Forest.ipynb` | Ensemble methods, feature importance |
| `03_Class_Imbalance.ipynb` | SMOTE, class_weight, recall vs precision tradeoff |
| `04_Feature_Engineering.ipynb` | Encoding, scaling, selection |
| `05_ML_Pipelines.ipynb` | Scikit-learn Pipeline, cleaner workflows |
| `06_Hyperparameter_Tuning.ipynb` | GridSearchCV, RandomizedSearchCV |
| `07_Clustering.ipynb` | K-Means, unsupervised learning intro |
| `Week7_Exercises.ipynb` | Practice problems |
| `📁 Project/` | Week 7 project brief |

---

## 📖 Key Concepts

### Random Forest
```python
from sklearn.ensemble import RandomForestClassifier

rf = RandomForestClassifier(n_estimators=100, random_state=42)
rf.fit(X_train, y_train)

# Feature importance
import pandas as pd
importance = pd.Series(rf.feature_importances_, index=X.columns)
importance.sort_values().plot(kind='barh')
```

### Handling Class Imbalance
```python
# Option 1: class_weight
rf = RandomForestClassifier(class_weight='balanced')

# Option 2: prioritize recall for minority class
from sklearn.metrics import classification_report
# Focus on recall for the attack/fraud class
print(classification_report(y_test, preds, target_names=['Benign', 'Attack']))
```

### ML Pipeline
```python
from sklearn.pipeline import Pipeline
from sklearn.preprocessing import StandardScaler

pipeline = Pipeline([
    ('scaler', StandardScaler()),
    ('model', RandomForestClassifier())
])

pipeline.fit(X_train, y_train)
print(pipeline.score(X_test, y_test))
```

---

## 🚀 Week 7 Project
**📁 See `Project/` folder**

**Project: Network Intrusion Detection System (Mini)**
- Classify network traffic as BENIGN or ATTACK
- Use Random Forest with proper evaluation metrics
- Focus on ATTACK-class recall — a missed attack is worse than a false alarm
- This is inspired by real-world ML security systems!

---

## 📝 Assignment
Complete `Week7_Exercises.ipynb` AND the project.
