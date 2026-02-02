# Feature Engineering in Machine Learning

## 1. What is Feature Engineering?
Feature Engineering is the process of creating, selecting, and transforming features to improve machine learning model performance.

Good features matter more than complex models.

---

## 2. Why Feature Engineering is Important
- Improves model accuracy
- Reduces overfitting
- Speeds up training
- Enhances interpretability

---

## 3. Types of Feature Engineering

### 3.1 Feature Creation
- Polynomial features
- Interaction features
- Domain-based features
- Date & time features

---

### 3.2 Feature Transformation
- Log transformation
- Power transformation
- Scaling & normalization

---

### 3.3 Feature Selection
Removing irrelevant or redundant features.

#### Methods:
- Filter Methods (Correlation, Chi-square)
- Wrapper Methods (RFE)
- Embedded Methods (Lasso, Tree-based)

---

### 3.4 Feature Extraction
Transforming data into a new feature space.

Examples:
- PCA
- t-SNE
- Autoencoders

---

## 4. Polynomial Features
Used when the relationship between features and target is non-linear.

Risk:
- Overfitting
- Curse of dimensionality

---

## 5. Dimensionality Reduction

### Why Reduce Dimensions?
- Reduces noise
- Improves generalization
- Faster training

### Common Techniques:
- PCA
- t-SNE
- UMAP

---

## 6. Correlation Analysis
Helps identify redundant features.

High correlation → multicollinearity → unstable models.

---

## 7. Feature Importance
Determines which features contribute most to predictions.

Methods:
- Tree-based importance
- Permutation importance
- SHAP values

---

## 8. Feature Engineering Pipeline
- Create features
- Select relevant features
- Scale features
- Validate impact

---

## 9. Common Mistakes
- Creating too many features
- Data leakage
- Ignoring domain knowledge
- Not validating feature impact

---

## 10. Interview Questions
1. Feature selection vs extraction?
2. When should we use PCA?
3. How does multicollinearity affect models?
4. Polynomial features pros & cons?
5. How do tree models handle features?
