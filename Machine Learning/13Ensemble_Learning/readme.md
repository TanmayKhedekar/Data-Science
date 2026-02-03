# Ensemble Learning (Boosting)

## 1. What is Ensemble Learning?
Ensemble Learning combines **multiple weak learners** to create a **strong learner**.

Core idea:
> Many weak models together outperform a single strong model.

---

## 2. Why Ensemble Learning?
Single models often suffer from:
- High bias
- High variance
- Limited representation power

Ensembles improve:
- Accuracy
- Robustness
- Generalization

---

## 3. Types of Ensemble Learning

### 3.1 Bagging (Bootstrap Aggregation)
- Trains models independently
- Reduces variance
- Example: Random Forest

---

### 3.2 Boosting (Main Focus)
- Trains models sequentially
- Each model corrects previous errors
- Reduces bias

---

### 3.3 Stacking
- Combines predictions using a meta-model
- More complex, higher risk of overfitting

---

## 4. Boosting — Core Idea
Boosting focuses on **hard-to-predict samples** by:
- Increasing their importance
- Forcing later models to learn difficult cases

---

## 5. AdaBoost (Adaptive Boosting)

### How AdaBoost Works
1. Assign equal weights to all samples
2. Train weak learner (usually decision stump)
3. Increase weights of misclassified samples
4. Train next learner on updated weights
5. Combine learners using weighted voting

---

### Key Characteristics
- Very sensitive to noise
- Works best with clean data
- Uses exponential loss

---

## 6. Gradient Boosting

### Core Idea
Gradient Boosting builds models **sequentially** where each model:
- Learns the **residual errors** of the previous model
- Optimizes a loss function using gradient descent

---

### Why Gradient Boosting is Powerful
- Works with any differentiable loss function
- Handles complex non-linear patterns
- Strong performance on tabular data

---

## 7. Gradient Boosting vs AdaBoost

| Aspect | AdaBoost | Gradient Boosting |
|------|---------|------------------|
| Error focus | Misclassified samples | Residual errors |
| Loss | Exponential | Any differentiable |
| Noise sensitivity | High | Lower |
| Flexibility | Low | High |

---

## 8. Important Hyperparameters (Boosting)

- `n_estimators` → number of trees
- `learning_rate` → contribution of each tree
- `max_depth` → tree complexity
- `subsample` → randomness (regularization)

---

## 9. Overfitting in Boosting
Boosting **can overfit** if:
- Too many estimators
- High learning rate
- Deep trees

Mitigation:
- Lower learning rate
- Early stopping
- Shallow trees

---

## 10. Advantages
- Very high accuracy
- Handles complex patterns
- Strong default choice for tabular data

---

## 11. Disadvantages
- Slower training
- Harder to tune
- Less interpretable

---

## 12. When to Use Boosting
- Structured/tabular datasets
- Medium-sized datasets
- When accuracy matters most

---

## 13. Common Mistakes
- Using large learning rate
- Too deep trees
- Ignoring early stopping
- Not tuning hyperparameters

---

## 14. Interview Questions
1. Bagging vs Boosting?
2. Why Boosting reduces bias?
3. AdaBoost vs Gradient Boosting?
4. Role of learning rate?
5. Why boosting overfits?
