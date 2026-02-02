# K-Nearest Neighbors (KNN)

## 1. What is KNN?
K-Nearest Neighbors (KNN) is a **supervised, non-parametric, instance-based** learning algorithm used for **classification and regression**.

KNN does not learn an explicit model — it memorizes the training data.

---

## 2. How KNN Works
1. Choose a value of K
2. Calculate distance between test point and all training points
3. Select K nearest neighbors
4. Perform:
   - Majority voting (classification)
   - Average (regression)

---

## 3. Distance Metrics

### Common Distance Metrics
- **Euclidean Distance**  
- **Manhattan Distance**
- **Minkowski Distance**
- **Cosine Similarity**

Choice of distance affects performance.

---

## 4. Choosing the Value of K
- Small K → overfitting (high variance)
- Large K → underfitting (high bias)

Rule of thumb:
- Start with K = √n
- Use cross-validation to choose K

---

## 5. Feature Scaling (VERY IMPORTANT)
KNN is **distance-based**.

If features are not scaled:
- Large-scale features dominate
- Distance becomes meaningless

Always apply:
- StandardScaler
- MinMaxScaler

---

## 6. Classification vs Regression
- **KNN Classification:** majority vote
- **KNN Regression:** mean of neighbors

---

## 7. Advantages
- Simple and intuitive
- No training phase
- Works well on small datasets

---

## 8. Disadvantages
- Slow prediction (O(n))
- High memory usage
- Sensitive to noise and scale
- Not suitable for large datasets

---

## 9. When to Use KNN
- Small datasets
- Low dimensional data
- Baseline model

---

## 10. Common Mistakes
- Not scaling features
- Choosing K arbitrarily
- Using KNN on large datasets
- Ignoring curse of dimensionality

---

## 11. Interview Questions
1. Why is KNN called a lazy learner?
2. Effect of K on bias-variance?
3. Why scaling is mandatory?
4. KNN vs Logistic Regression?
5. Time complexity of KNN?
