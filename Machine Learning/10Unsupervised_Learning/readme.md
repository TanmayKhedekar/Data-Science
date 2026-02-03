# Unsupervised Learning

## 1. What is Unsupervised Learning?
Unsupervised Learning is a type of Machine Learning where the model learns patterns from **unlabeled data**.
There is no target variable — the goal is to discover hidden structure.

---

## 2. Why Unsupervised Learning?
- No labeled data available
- Exploratory data analysis
- Pattern discovery
- Data compression
- Anomaly detection

---

## 3. Main Types of Unsupervised Learning
1. Clustering
2. Dimensionality Reduction
3. Anomaly Detection
4. Association Rule Mining

---

## 4. Clustering
Clustering groups similar data points together based on similarity or distance.

### Common Clustering Algorithms
- K-Means
- Hierarchical Clustering
- DBSCAN

---

## 5. K-Means Clustering

### How K-Means Works
1. Choose K (number of clusters)
2. Initialize centroids
3. Assign points to nearest centroid
4. Update centroids
5. Repeat until convergence

### Assumptions
- Clusters are spherical
- Similar size clusters

### Choosing K
- Elbow Method
- Silhouette Score

---

## 6. Hierarchical Clustering
- Builds a tree-like structure (dendrogram)
- Agglomerative (bottom-up)
- Divisive (top-down)

Pros:
- No need to choose K initially

Cons:
- Computationally expensive

---

## 7. DBSCAN (Density-Based Clustering)
- Groups dense regions
- Identifies noise/outliers

Key Parameters:
- `eps` → neighborhood radius
- `min_samples` → minimum points

Advantages:
- Finds arbitrary shaped clusters
- Handles noise well

---

## 8. Dimensionality Reduction
Reduces number of features while preserving information.

Why?
- Curse of dimensionality
- Visualization
- Faster training

---

## 9. Principal Component Analysis (PCA)
- Linear dimensionality reduction
- Maximizes variance
- Creates orthogonal components

Trade-off:
- Reduced interpretability

---

## 10. Applications
- Customer segmentation
- Market basket analysis
- Image compression
- Anomaly detection
- Topic modeling

---

## 11. Common Mistakes
- Wrong choice of K
- Using K-Means on non-spherical data
- Ignoring feature scaling
- Misinterpreting clusters

---

## 12. Interview Questions
1. Supervised vs Unsupervised learning?
2. How does K-Means choose clusters?
3. What are limitations of K-Means?
4. DBSCAN vs K-Means?
5. When to use PCA?
