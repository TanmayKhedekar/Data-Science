# Model Evaluation in Machine Learning

## 1. What is Model Evaluation?
Model Evaluation is the process of assessing how well a machine learning model performs on **unseen data**.

A good model:
- Learns patterns (not noise)
- Generalizes well
- Performs consistently

---

## 2. Why Model Evaluation is Critical
- Prevents overfitting
- Enables fair model comparison
- Guides hyperparameter tuning
- Ensures real-world reliability

---

## 3. Types of Evaluation Scenarios
- Regression
- Classification
- Imbalanced classification

---

## 4. Regression Evaluation Metrics

### 4.1 Mean Absolute Error (MAE)
MAE = (1/n) Σ |y − ŷ|

- Measures average absolute error
- Less sensitive to outliers

---

### 4.2 Mean Squared Error (MSE)
MSE = (1/n) Σ (y − ŷ)²

- Penalizes large errors
- Differentiable → optimization-friendly

---

### 4.3 Root Mean Squared Error (RMSE)
RMSE = √MSE

- Same unit as target variable
- Easier to interpret

---

### 4.4 R² Score (Coefficient of Determination)
Measures how much variance is explained by the model.

- 1 → perfect fit
- 0 → predicts mean
- < 0 → worse than baseline

---

## 5. Classification Evaluation Metrics

---

### 5.1 Confusion Matrix
| Actual \ Predicted | Positive | Negative |
|--------------------|----------|----------|
| Positive | TP | FN |
| Negative | FP | TN |

---

### 5.2 Accuracy
Accuracy = (TP + TN) / Total

⚠️ Misleading for **imbalanced datasets**

---

### 5.3 Precision
Precision = TP / (TP + FP)

Use when:
- False positives are costly (spam, fraud)

---

### 5.4 Recall
Recall = TP / (TP + FN)

Use when:
- False negatives are costly (disease detection)

---

### 5.5 F1-Score
F1 = 2 × (Precision × Recall) / (Precision + Recall)

Balances precision and recall.

---

### 5.6 ROC Curve & AUC
- ROC → TPR vs FPR
- AUC → probability that model ranks positive higher than negative

AUC = 0.5 → random  
AUC = 1.0 → perfect

---

## 6. Threshold Selection
Default threshold = 0.5  
Changing threshold impacts:
- Precision
- Recall

Used in:
- Fraud detection
- Medical diagnosis

---

## 7. Evaluation for Imbalanced Data
Avoid:
- Accuracy

Prefer:
- Precision
- Recall
- F1-score
- ROC-AUC
- PR-AUC

---

## 8. Bias–Variance Tradeoff

- **High Bias** → Underfitting
- **High Variance** → Overfitting

Goal:
- Balance both for best generalization

---

## 9. Cross-Validation

### Why?
- Single train-test split is unreliable

### K-Fold Cross-Validation
- Data split into K folds
- Each fold used as test once
- Average performance reported

---

## 10. Model Comparison
Always compare models on:
- Same dataset
- Same split
- Same metric

---

## 11. Common Mistakes
- Using accuracy blindly
- Evaluating on training data
- Ignoring data leakage
- Comparing models unfairly

---

## 12. Interview Questions
1. Why accuracy fails on imbalanced data?
2. Precision vs Recall?
3. When to use ROC-AUC?
4. What does R² < 0 mean?
5. Bias vs variance?
