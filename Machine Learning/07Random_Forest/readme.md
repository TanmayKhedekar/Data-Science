# Random Forest

## 1. What is Random Forest?
Random Forest is an **ensemble learning algorithm** that builds **multiple Decision Trees** and combines their predictions to improve accuracy and reduce overfitting.

It works on the principle of **Bagging (Bootstrap Aggregation)**.

---

## 2. Why Random Forest?
Decision Trees:
- Overfit easily
- High variance

Random Forest:
- Reduces variance
- Improves generalization
- More robust and stable

---

## 3. How Random Forest Works
1. Create multiple bootstrap samples from the dataset
2. Train a Decision Tree on each sample
3. At each split, consider only a random subset of features
4. Aggregate predictions:
   - Majority voting (classification)
   - Mean (regression)

---

## 4. Bagging (Bootstrap Aggregation)
- Random sampling **with replacement**
- Each tree sees slightly different data
- Trees are **decorrelated**

---

## 5. Random Feature Selection
At each split:
- Only a subset of features is considered
- Prevents dominant features
- Increases diversity among trees

---

## 6. Random Forest for Classification vs Regression
- **Classifier:** majority vote
- **Regressor:** average of predictions

---

## 7. Hyperparameters (Very Important)
- `n_estimators` → number of trees
- `max_depth` → depth of trees
- `min_samples_split`
- `min_samples_leaf`
- `max_features`

---

## 8. Feature Importance
Random Forest provides feature importance based on:
- Gini importance
- Reduction in impurity

Helps in:
- Feature selection
- Model interpretability

---

## 9. Advantages
- Handles non-linearity
- Reduces overfitting
- Works well with large datasets
- No feature scaling required

---

## 10. Disadvantages
- Less interpretable than a single tree
- Slower training
- Large memory usage

---

## 11. When to Use Random Forest
- Strong baseline model
- Tabular data
- Non-linear relationships
- Feature importance needed

---

## 12. Common Mistakes
- Too many trees without tuning
- Very deep trees
- Ignoring feature importance
- Using RF when speed is critical

---

## 13. Interview Questions
1. Why Random Forest over Decision Tree?
2. What is bagging?
3. How Random Forest reduces overfitting?
4. Meaning of `max_features`?
5. Random Forest vs Gradient Boosting?
