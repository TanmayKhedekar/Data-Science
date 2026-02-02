# Decision Trees

## 1. What is a Decision Tree?
A Decision Tree is a **supervised learning algorithm** used for both **classification and regression**.
It models decisions as a tree structure where:
- Internal nodes → feature tests
- Branches → outcomes
- Leaf nodes → predictions

---

## 2. How Decision Trees Work
1. Select the best feature to split the data
2. Split the dataset into subsets
3. Repeat recursively for each subset
4. Stop when a stopping condition is met

---

## 3. Splitting Criteria (Impurity Measures)

### 3.1 Gini Impurity
Gini = 1 − Σ(pᵢ²)

- Measures how often a randomly chosen element is incorrectly classified
- Used by CART algorithm
- Faster to compute

---

### 3.2 Entropy
Entropy = −Σ(pᵢ log₂ pᵢ)

- Measures randomness
- Used in ID3 and C4.5

---

### 3.3 Information Gain
Information Gain = Parent Entropy − Weighted Child Entropy

Higher gain → better split.

---

## 4. Decision Tree for Classification vs Regression
- **Classification Tree:** predicts class labels
- **Regression Tree:** predicts continuous values using mean squared error

---

## 5. Stopping Criteria
- Maximum depth reached
- Minimum samples per leaf
- Node becomes pure
- No further gain possible

---

## 6. Overfitting in Decision Trees
Decision Trees easily overfit because:
- They can grow very deep
- They memorize training data

---

## 7. Pruning Techniques

### 7.1 Pre-Pruning (Early Stopping)
- max_depth
- min_samples_split
- min_samples_leaf

### 7.2 Post-Pruning
- Cost complexity pruning (ccp_alpha)

---

## 8. Advantages
- Easy to understand & visualize
- No feature scaling required
- Handles non-linear relationships
- Works with mixed data types

---

## 9. Disadvantages
- High variance
- Overfitting
- Unstable to small data changes

---

## 10. When to Use Decision Trees
- Interpretability is required
- Baseline model
- Feature importance needed

---

## 11. Common Mistakes
- Allowing unlimited depth
- Ignoring pruning
- Using trees alone for complex problems
- Small datasets with deep trees

---

## 12. Interview Questions
1. Gini vs Entropy?
2. Why do Decision Trees overfit?
3. What is pruning?
4. Are Decision Trees affected by scaling?
5. How do trees handle non-linearity?
