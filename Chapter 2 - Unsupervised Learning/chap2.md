# 🧩 Chapter 2: Unsupervised Learning (Pattern Detectives)

> “When no answers are given, patterns become the answers.”

---

# 📌 1. What is Unsupervised Learning?

Unsupervised Learning is a type of Machine Learning where the model is trained on **unlabeled data**.

- No predefined outputs
- Model discovers hidden structures and relationships

\[
\text{Given } X \Rightarrow \text{Find patterns / structure}
\]

---

# 🎯 2. Core Idea

The model acts like a **detective**:

- Finds similarities
- Groups data
- Identifies relationships

| Step | Description          |
| ---- | -------------------- |
| 1    | Input raw data       |
| 2    | Analyze similarities |
| 3    | Detect patterns      |
| 4    | Group or associate   |

---

# 🔀 3. Types of Unsupervised Learning

## 📊 3.1 Clustering

### 📌 Definition:

Grouping similar data points together

### 📍 Examples:

- Customer segmentation
- Image grouping
- Document classification

---

## 🔗 3.2 Association Rules

### 📌 Definition:

Finding relationships between items

### 📍 Examples:

- Market basket analysis
- Product recommendations

---

# ⚖️ 4. Clustering vs Association

| Feature | Clustering         | Association        |
| ------- | ------------------ | ------------------ |
| Goal    | Group similar data | Find relationships |
| Output  | Clusters           | Rules              |
| Example | Customer groups    | Bread → Milk       |

---

# 🧮 5. K-Means Clustering

## 📌 Objective:

Divide data into **K clusters**

## 🔁 Algorithm Steps:

1. Choose number of clusters \(K\)
2. Initialize centroids
3. Assign points to nearest centroid
4. Recalculate centroids
5. Repeat until convergence

---

## 📐 Distance Formula (Euclidean)

\[
d = \sqrt{(x_1 - x_2)^2 + (y_1 - y_2)^2}
\]

---

## 📊 Objective Function (WCSS)

\[
WCSS = \sum (x_i - \mu_k)^2
\]

Where:

- \( \mu_k \) = centroid of cluster

---

# 📉 6. Elbow Method

Used to find optimal number of clusters.

### 📌 Idea:

Plot:

- X-axis → Number of clusters (K)
- Y-axis → WCSS

Choose K where curve bends (elbow point)

---

# 🔄 7. K-Means vs K-Medoids

| Feature     | K-Means                 | K-Medoids         |
| ----------- | ----------------------- | ----------------- |
| Center      | Mean (not actual point) | Actual data point |
| Sensitivity | Sensitive to outliers   | More robust       |
| Speed       | Faster                  | Slower            |

---

# 🔗 8. Association Rule Learning

## 📌 Goal:

Find rules like:

\[
X \Rightarrow Y
\]

Example:
\[
\{Bread, Milk\} \Rightarrow \{Eggs\}
\]

---

## 📏 Key Metrics

### 📊 Support

\[
Support(X) = \frac{\text{Transactions containing X}}{\text{Total Transactions}}
\]

---

### 📊 Confidence

\[
Confidence(X \Rightarrow Y) = \frac{Support(X \cup Y)}{Support(X)}
\]

---

# 🧠 9. Apriori Algorithm

## 📌 Principle:

“If an itemset is frequent, all its subsets are also frequent.”

---

## 🔁 Steps:

1. Generate candidate itemsets
2. Remove infrequent ones
3. Repeat until no new itemsets

---

# ⚡ 10. ECLAT Algorithm

## 📌 Key Idea:

Uses **vertical data format**

- Stores Transaction IDs (TID)
- Uses intersection to find support

---

## 📊 Comparison

| Feature     | Apriori       | ECLAT       |
| ----------- | ------------- | ----------- |
| Data Format | Horizontal    | Vertical    |
| Speed       | Slower        | Faster      |
| Approach    | Breadth-first | Depth-first |

---

# ⚙️ 11. Important Concepts

## 🔹 Centroid

Center of a cluster:
\[
\mu = \frac{1}{n} \sum x_i
\]

---

## 🔹 Similarity Measure

Used to compare data points:

- Euclidean distance
- Manhattan distance
- Cosine similarity

---

# 🧪 12. Real-World Applications

| Domain       | Use Case                |
| ------------ | ----------------------- |
| Marketing    | Customer segmentation   |
| Retail       | Product recommendations |
| Finance      | Fraud pattern detection |
| Social Media | User behavior grouping  |

---

# 🧠 13. Intuition Summary

- No labels → model discovers patterns
- Groups similar items
- Finds relationships in data

---

# 🔥 14. Quick Recap

- Unsupervised Learning = No labeled data
- Two main types:
  - Clustering
  - Association Rules
- Algorithms:
  - K-Means
  - Apriori
  - ECLAT

---

# 💡 15. Practice Ideas

- Segment customers using K-Means
- Build recommendation system
- Analyze shopping patterns

---

# 🚀 Final Thought

Unsupervised Learning helps uncover **hidden insights** that humans might miss.

---
