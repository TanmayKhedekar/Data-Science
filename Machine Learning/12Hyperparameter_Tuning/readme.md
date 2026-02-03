# Hyperparameter Tuning in Machine Learning

## 1. What are Hyperparameters?
Hyperparameters are **external configuration values** set **before training** a model.
They control how a model learns but are **not learned from data**.

Examples:
- Learning rate
- Number of neighbors (K in KNN)
- Max depth of a tree
- Number of estimators in Random Forest

---

## 2. Hyperparameters vs Parameters

| Aspect | Parameters | Hyperparameters |
|-----|-----------|----------------|
| Learned from data | Yes | No |
| Set before training | No | Yes |
| Example | Weights, bias | K, learning rate |

---

## 3. Why Hyperparameter Tuning is Important
- Improves model performance
- Controls bias–variance tradeoff
- Prevents overfitting and underfitting
- Makes models generalize better

---

## 4. Bias–Variance Tradeoff (Revisited)

- **High Bias** → underfitting → model too simple
- **High Variance** → overfitting → model too complex

Hyperparameters directly control this balance.

---

## 5. Manual Tuning
- Trial and error
- Uses intuition
- Not scalable
- Not reproducible

---

## 6. Grid Search

### Idea
Try **all possible combinations** of hyperparameters.

### Pros
- Exhaustive
- Guarantees best combination (within grid)

### Cons
- Very slow
- Computationally expensive

---

## 7. Random Search

### Idea
Randomly sample combinations from parameter space.

### Pros
- Faster than Grid Search
- Often finds good solutions
- Scales well

### Cons
- No guarantee of optimal solution

---

## 8. Bayesian Optimization (Conceptual)
- Uses probability model to choose next best parameters
- Learns from past evaluations
- More efficient than grid/random

Examples:
- Gaussian Processes
- Tree-structured Parzen Estimators (TPE)

---

## 9. Cross-Validation in Tuning
Hyperparameter tuning must be done using **cross-validation** to:
- Avoid overfitting to validation set
- Get stable performance estimates

---

## 10. Nested Cross-Validation (Advanced)
- Outer loop → model evaluation
- Inner loop → hyperparameter tuning
- Prevents overly optimistic results

---

## 11. Early Stopping
Stops training when performance stops improving.

Used in:
- Gradient Boosting
- Neural Networks

Benefits:
- Saves time
- Prevents overfitting

---

## 12. Common Hyperparameters by Algorithm

### KNN
- n_neighbors
- distance metric

### Decision Tree
- max_depth
- min_samples_split
- min_samples_leaf

### Random Forest
- n_estimators
- max_depth
- max_features

### SVM
- C
- gamma
- kernel

---

## 13. Common Mistakes
- Tuning on test data ❌
- Using too large grids ❌
- Ignoring cross-validation ❌
- Optimizing wrong metric ❌

---

## 14. Interview Questions
1. Grid Search vs Random Search?
2. Why cross-validation is needed in tuning?
3. What is nested CV?
4. How hyperparameters affect bias–variance?
5. Why Random Search often beats Grid Search?
