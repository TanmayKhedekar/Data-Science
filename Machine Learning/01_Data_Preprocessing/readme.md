# Data Preprocessing in Machine Learning

## 1. What is Data Preprocessing?
Data Preprocessing is the process of cleaning, transforming, and preparing raw data so that it can be effectively used by machine learning models.

High-quality data leads to better models than complex algorithms with poor data.

---

## 2. Why Data Preprocessing is Important
- Real-world data is messy
- Missing values affect learning
- Different scales bias models
- Categorical data must be encoded
- Reduces noise and improves accuracy

---

## 3. Types of Data Problems
- Missing values
- Duplicate records
- Outliers
- Inconsistent formats
- Categorical variables
- Feature scale differences

---

## 4. Handling Missing Values

### 4.1 Types of Missing Data
- MCAR (Missing Completely at Random)
- MAR (Missing at Random)
- MNAR (Missing Not at Random)

### 4.2 Techniques
- Remove rows or columns
- Mean / Median / Mode imputation
- Forward / Backward fill
- Model-based imputation

---

## 5. Handling Categorical Data

### 5.1 Label Encoding
- Converts categories into integers
- Suitable for ordinal data

### 5.2 One-Hot Encoding
- Creates binary columns
- Avoids ordinal bias
- Increases dimensionality

---

## 6. Feature Scaling

### 6.1 Why Scaling Matters
Distance-based models are sensitive to scale:
- KNN
- SVM
- K-Means
- Gradient Descent-based models

### 6.2 Scaling Techniques
- Min-Max Scaling
- Standardization (Z-score)
- Robust Scaling

---

## 7. Handling Outliers

### 7.1 What are Outliers?
Data points that significantly differ from others.

### 7.2 Detection Methods
- Boxplot (IQR method)
- Z-score
- Visualization

### 7.3 Treatment
- Remove
- Cap (Winsorization)
- Transform

---

## 8. Train-Test Split
Splitting data ensures the model is evaluated on unseen data.

Typical splits:
- 70–30
- 80–20

Why?
- Prevents overfitting
- Simulates real-world performance

---

## 9. Data Leakage (Very Important)
Data leakage occurs when information from the test set leaks into the training process.

Examples:
- Scaling before train-test split
- Using future data

---

## 10. Best Practices
- Always preprocess after splitting
- Visualize data before cleaning
- Use pipelines
- Keep raw data unchanged

---

## 11. Common Interview Questions
1. Mean vs Median imputation?
2. When should we remove missing values?
3. Why scaling is needed?
4. What is data leakage?
5. Which models need scaling?
