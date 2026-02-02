# Support Vector Machine (SVM)

## 1. What is SVM?
Support Vector Machine (SVM) is a **supervised learning algorithm** used for **classification and regression**.
It works by finding an **optimal hyperplane** that best separates data points of different classes.

The goal is to **maximize the margin** between classes.

---

## 2. Key Concepts

### 2.1 Hyperplane
A decision boundary that separates classes.
- In 2D → line
- In 3D → plane
- In higher dimensions → hyperplane

---

### 2.2 Margin
Distance between the hyperplane and the nearest data points from each class.

- Larger margin → better generalization

---

### 2.3 Support Vectors
The **closest data points** to the hyperplane.
These points **define the decision boundary**.

---

## 3. Hard Margin vs Soft Margin

### Hard Margin SVM
- No misclassification allowed
- Works only when data is perfectly separable

### Soft Margin SVM
- Allows misclassification
- Uses a penalty parameter `C`
- Works well on real-world noisy data

---

## 4. Regularization Parameter (C)
- Controls trade-off between:
  - Maximizing margin
  - Minimizing classification error

- Large C → low bias, high variance (overfitting)
- Small C → high bias, low variance (underfitting)

---

## 5. Kernel Trick (Very Important)
SVM can solve **non-linear problems** using kernels.

Kernels implicitly map data to higher dimensions.

### Common Kernels
- Linear
- Polynomial
- RBF (Gaussian)
- Sigmoid

---

## 6. RBF Kernel
Most widely used kernel.

Key parameter:
- **Gamma (γ)** → controls influence of single training points

High gamma → overfitting  
Low gamma → underfitting

---

## 7. SVM for Classification vs Regression
- **SVC** → classification
- **SVR** → regression

---

## 8. Feature Scaling (MANDATORY)
SVM is **distance-based**.

Without scaling:
- Dominant features distort margin
- Poor performance

Always apply:
- StandardScaler
- MinMaxScaler

---

## 9. Advantages
- Effective in high-dimensional spaces
- Works well with small datasets
- Strong theoretical foundation

---

## 10. Disadvantages
- Computationally expensive
- Hard to tune
- Less interpretable
- Not suitable for very large datasets

---

## 11. When to Use SVM
- Small to medium datasets
- Clear margin of separation
- High-dimensional data (text, bioinformatics)

---

## 12. Common Mistakes
- Not scaling features
- Wrong kernel choice
- Poor tuning of C and gamma
- Using SVM on very large datasets

---

## 13. Interview Questions
1. What are support vectors?
2. Why scaling is mandatory for SVM?
3. Explain kernel trick.
4. Difference between C and gamma?
5. SVM vs Logistic Regression?
