# Naive Bayes

## 1. What is Naive Bayes?
Naive Bayes is a **supervised probabilistic classification algorithm** based on **Bayes’ Theorem**.

It is called “naive” because it assumes that **all features are independent**, which is rarely true in real life.

---

## 2. Bayes’ Theorem

P(Class | Features) =
P(Features | Class) × P(Class)
--------------------------------
        P(Features)

Where:
- P(Class | Features) → Posterior
- P(Features | Class) → Likelihood
- P(Class) → Prior
- P(Features) → Evidence

---

## 3. Why Naive Bayes Works (Despite Being Naive)
- Independence assumption simplifies computation
- Works surprisingly well in high-dimensional data
- Especially effective for text classification

---

## 4. Types of Naive Bayes

### 4.1 Gaussian Naive Bayes
- Assumes features follow a normal distribution
- Used for continuous data

---

### 4.2 Multinomial Naive Bayes
- Used for discrete counts
- Common in NLP (word frequencies)

---

### 4.3 Bernoulli Naive Bayes
- Binary features (0 or 1)
- Presence/absence of features

---

## 5. How Naive Bayes Classifies
1. Calculate prior probabilities
2. Calculate likelihood for each feature
3. Multiply probabilities
4. Choose class with highest posterior probability

---

## 6. Log Probability Trick
Instead of multiplying probabilities:
- Take logarithm
- Prevents numerical underflow
- Converts multiplication into addition

---

## 7. Advantages
- Very fast
- Works well with small datasets
- Performs well in text classification
- Requires less training data

---

## 8. Disadvantages
- Strong independence assumption
- Poor performance when features are correlated
- Zero probability problem

---

## 9. Zero Probability Problem & Laplace Smoothing
If a feature never appears in a class:
- Probability becomes zero

Solution:
- **Laplace (Add-One) Smoothing**

---

## 10. When to Use Naive Bayes
- Spam filtering
- Sentiment analysis
- Document classification
- Medical diagnosis (baseline)

---

## 11. Common Mistakes
- Using Gaussian NB on categorical data
- Ignoring feature distributions
- Not using smoothing
- Expecting high accuracy on correlated features

---

## 12. Interview Questions
1. Why is Naive Bayes called naive?
2. Explain Bayes’ theorem.
3. Gaussian vs Multinomial NB?
4. What is Laplace smoothing?
5. Why NB works well for text?
