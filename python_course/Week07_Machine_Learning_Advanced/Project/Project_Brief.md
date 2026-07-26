# 🔐 Week 7 Project — Network Intrusion Detection System (Mini IDS)

## Overview
You will build a simplified **Machine Learning-based Intrusion Detection System (IDS)** — a real-world cybersecurity tool that classifies network traffic as either **BENIGN** or **ATTACK**.

This is inspired by real production security systems used in organizations worldwide.

---

## Dataset
**CICIDS 2017 (subset)** — Canadian Institute for Cybersecurity Intrusion Detection dataset.

Download instructions in `starter_notebook.ipynb`

Features include: packet size, duration, protocol, flow bytes/sec, flags, etc.
Target: `Label` — BENIGN or attack type (we'll simplify to binary)

---

## Tasks

### Part 1 — Data Preparation (20 pts)
1. Load the dataset
2. Drop null values and infinite values (`np.inf`)
3. Encode the label column: BENIGN = 0, everything else = 1
4. Split into features (X) and target (y)
5. Apply train/test split (80/20)

### Part 2 — Model Building (30 pts)
1. Train a **Random Forest Classifier**
2. Train a **Logistic Regression** model
3. Compare both models

### Part 3 — Evaluation (30 pts)
1. Print the classification report for both models
2. Plot the confusion matrix
3. **Focus on ATTACK class recall** — explain why this matters more than accuracy in security

### Part 4 — Insights (20 pts)
1. Which model performed better and why?
2. What features are most important (use feature_importances_)?
3. What are the limitations of your model?

---

## Key Security Concept
> In cybersecurity, **a missed attack (False Negative) is always more costly than a false alarm (False Positive)**. This is why we optimize for RECALL on the attack class, not just overall accuracy.

---

## Submission
- Completed `.ipynb` notebook with all cells run
- A short paragraph (5-10 sentences) reflection on what you learned

**Due:** Before Week 8 (Capstone)

---

## Grading
| Criteria | Points |
|----------|--------|
| Data preparation correct | 20 |
| Both models trained & compared | 30 |
| Evaluation metrics correctly used | 30 |
| Quality of insights & reflection | 20 |
| **Total** | **100** |
