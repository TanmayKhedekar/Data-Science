# Linear Regression

## 1. What is Linear Regression?
Linear Regression is a **supervised learning algorithm** used to predict **continuous numerical values** by modeling the relationship between input features and a target variable.

The model assumes a linear relationship between inputs and output.

---

## 2. Types of Linear Regression
1. **Simple Linear Regression** – one independent variable  
2. **Multiple Linear Regression** – multiple independent variables  

---

## 3. Mathematical Representation

### Simple Linear Regression
y = wx + b

Where:
- y → predicted value
- x → input feature
- w → weight (slope)
- b → bias (intercept)

---

### Multiple Linear Regression
y = w₁x₁ + w₂x₂ + ... + wₙxₙ + b

---

## 4. Loss Function
Linear Regression uses **Mean Squared Error (MSE)**:

MSE = (1/n) Σ (yᵢ − ŷᵢ)²

Why MSE?
- Differentiable
- Penalizes large errors
- Works well with Gradient Descent

---

## 5. How the Model Learns (Gradient Descent)

Steps:
1. Initialize weights randomly
2. Predict output
3. Calculate loss
4. Compute gradients
5. Update weights
6. Repeat until convergence

Learning Rate controls step size.

---

## 6. Assumptions of Linear Regression
1. Linearity
2. Independence
3. Homoscedasticity
4. Normality of errors
5. No multicollinearity

Violation of assumptions → unreliable predictions.

---

## 7. Evaluation Metrics
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- R² Score

---

## 8. Advantages
- Simple and fast
- Highly interpretable
- Works well on small datasets

---

## 9. Disadvantages
- Sensitive to outliers
- Assumption-dependent
- Poor performance on non-linear data

---

## 10. Regularized Linear Regression
- **Ridge Regression** → L2 penalty
- **Lasso Regression** → L1 penalty
- **ElasticNet** → L1 + L2

Used to prevent overfitting.

---

## 11. Real-World Use Cases
- House price prediction
- Salary estimation
- Sales forecasting
- Risk analysis

---

## 12. Common Mistakes
- Ignoring assumptions
- Not scaling features
- Using R² alone
- Data leakage

---

## 13. Interview Questions
1. Why MSE instead of MAE?
2. Difference between Linear & Logistic Regression?
3. What happens if learning rate is too high?
4. When to use Ridge vs Lasso?
5. What does R² represent?
