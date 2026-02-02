# Logistic Regression

## 1. What is Logistic Regression?
Logistic Regression is a **supervised learning algorithm** used for **classification problems**, primarily **binary classification**.

Despite the name, Logistic Regression is a **classification algorithm**, not a regression algorithm.

---

## 2. Why Not Linear Regression for Classification?
Linear Regression:
- Outputs continuous values
- Can predict values < 0 or > 1

Classification requires:
- Probabilities between 0 and 1

Logistic Regression solves this using the **Sigmoid function**.

---

## 3. Sigmoid (Logistic) Function

σ(z) = 1 / (1 + e⁻ᶻ)

Properties:
- Output range: (0, 1)
- Converts linear output into probability

---

## 4. Mathematical Representation

z = w₁x₁ + w₂x₂ + ... + wₙxₙ + b  
ŷ = σ(z)

Where:
- ŷ → predicted probability
- Decision threshold (usually 0.5)

---

## 5. Decision Boundary
- A line (2D) or hyperplane (higher dimensions)
- Separates different classes
- Depends on weights and bias

---

## 6. Loss Function (Log Loss / Binary Cross-Entropy)

Loss = −[y log(ŷ) + (1 − y) log(1 − ŷ)]

Why not MSE?
- MSE leads to non-convex loss
- Cross-entropy is convex → better optimization

---

## 7. How the Model Learns
- Initialize weights
- Compute probabilities
- Calculate log loss
- Update weights using Gradient Descent
- Repeat until convergence

---

## 8. Types of Logistic Regression
1. **Binary Logistic Regression** (2 classes)
2. **Multinomial Logistic Regression** (more than 2 classes)
3. **One-vs-Rest (OvR)**

---

## 9. Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix

---

## 10. Advantages
- Simple & fast
- Outputs probabilities
- Interpretable coefficients

---

## 11. Disadvantages
- Assumes linear decision boundary
- Sensitive to outliers
- Struggles with complex patterns

---

## 12. Regularization
- **L1 (Lasso)** → feature selection
- **L2 (Ridge)** → reduces overfitting

---

## 13. Real-World Use Cases
- Spam detection
- Disease diagnosis
- Fraud detection
- Credit risk modeling

---

## 14. Common Mistakes
- Using accuracy on imbalanced data
- Not scaling features
- Wrong threshold selection
- Ignoring class imbalance

---

## 15. Interview Questions
1. Why use log loss instead of MSE?
2. How is Logistic Regression different from Linear Regression?
3. What is ROC-AUC?
4. What happens if threshold ≠ 0.5?
5. When does Logistic Regression fail?
