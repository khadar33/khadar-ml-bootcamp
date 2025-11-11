# 📘 Assignment 8 — Clustering (Unsupervised Learning)

**Author:** Ali Omar Abdi
**Project Type:** Academic Assignment — Machine Learning (Unsupervised Learning)

---

## 🧠 1. Introduction to Clustering

### What Is Clustering?

**Clustering** is one of the main techniques in **unsupervised learning**, where the goal is to **find natural patterns or groups** within a dataset **without using labels**.
In simple terms, clustering automatically groups data points that are **similar to each other** into the same cluster, while keeping **dissimilar points** in different clusters.

💡 **Example:**
Imagine a store with thousands of customers but no information about their buying types. Clustering helps group them into categories such as:

* “Frequent Shoppers”
* “Seasonal Buyers”
* “Low-Spending Customers”

This helps the business understand customer behavior and plan better marketing strategies.

---

### How Is Clustering Different from Supervised Learning?

| Feature       | Supervised Learning                         | Unsupervised Learning (Clustering)          |
| :------------ | :------------------------------------------ | :------------------------------------------ |
| **Data Type** | Uses **labeled data** (with known answers). | Uses **unlabeled data** (no answers given). |
| **Goal**      | Predict an output (e.g., spam or not spam). | Discover structure or patterns in the data. |
| **Example**   | Predicting house prices based on features.  | Grouping houses by price range or location. |

In supervised learning, we **train** the model using examples with correct outputs.
In clustering, there are **no answers to learn from** — the algorithm must find patterns **on its own**.

---

### Real-Life Examples

* **Clustering Example:** Grouping news articles by topic automatically.
* **Supervised Example:** Predicting whether an email is spam or not (using labeled training data).

---

## ⚙️ 2. Clustering Algorithms

There are many clustering methods, but three of the most common are:

---

### 🟢 2.1 K-Means Clustering

**How It Works:**

1. Choose the number of clusters (**k**).
2. Randomly place **k points** (called *centroids*) as cluster centers.
3. Assign each data point to the nearest centroid.
4. Recalculate each centroid’s position (average of its cluster).
5. Repeat steps 3–4 until the centroids don’t move much.

**Example Use:**
Used in **customer segmentation**, where companies divide customers into groups based on spending habits.

**Advantages:**

* Simple and fast for large datasets.
* Works well when clusters are round and well-separated.

**Limitations:**

* Must choose *k* before starting.
* Doesn’t handle irregular-shaped clusters or outliers well.

---

### 🟣 2.2 Hierarchical Clustering

**How It Works:**
Hierarchical clustering builds a tree of clusters, called a **dendrogram**.
It starts by treating every point as its own cluster and then **merges** the most similar clusters step by step until only one large cluster remains.

**Example Use:**
Used in **biology and genetics** to find relationships among species or genes.

**Advantages:**

* No need to predefine *k*.
* Gives a clear visual structure through a dendrogram.

**Limitations:**

* Slow and memory-intensive for large datasets.
* Once merged, clusters cannot be split again.

---

### 🔵 2.3 DBSCAN (Density-Based Spatial Clustering)

**How It Works:**
DBSCAN groups data points that are close together (dense regions) and labels isolated points as **noise** or **outliers**.
It uses two parameters:

* `eps` → maximum distance between two points in the same cluster.
* `min_samples` → minimum number of points to form a cluster.

**Example Use:**
Detecting unusual patterns such as **fraud detection** or **geographic data clustering**.

**Advantages:**

* Handles noise and outliers well.
* Can find clusters of any shape.

**Limitations:**

* Sensitive to the choice of `eps` and `min_samples`.
* Struggles when data has varying densities.

---

## 📈 3. Clustering Evaluation Metrics

Since clustering doesn’t use labels, we must use **internal metrics** to measure how good the clusters are.

| Metric                   | What It Measures                                                                    | What a “Good” Value Means                                                         | When to Use                               |
| :----------------------- | :---------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------- | :---------------------------------------- |
| **Elbow Method**         | Measures how compact the clusters are (total WCSS = Within-Cluster Sum of Squares). | The “elbow point” where improvement slows down indicates the best *k*.            | Choosing *k* for K-Means.                 |
| **Silhouette Score**     | Measures how well-separated clusters are.                                           | A value close to **1.0** means good separation; 0 or below means poor clustering. | Evaluating cluster quality.               |
| **Davies–Bouldin Index** | Measures similarity between clusters.                                               | A **lower value** means better separation between clusters.                       | Comparing different models or parameters. |

---

## ⚠️ 4. Challenges in Clustering

Clustering can be harder than supervised learning because **there are no correct labels** to check against.
We rely on metrics and visualizations to judge quality.

### Common Challenges

1. **Choosing the Number of Clusters (k):**
   It’s often unclear how many natural groups exist. The Elbow Method helps, but the result is sometimes subjective.

2. **Handling Noise and Outliers:**
   Outliers can pull cluster centers away from the true mean (especially in K-Means).

3. **High-Dimensional Data:**
   When datasets have many features, clusters become hard to visualize and interpret.

---

## 🌍 5. Real-World Case Study — Customer Segmentation

### Project Goal

An e-commerce company wanted to improve marketing by sending **personalized offers** to different customer groups.

### Data Used

The dataset included **Recency (R)**, **Frequency (F)**, and **Monetary Value (M)** — known as **RFM analysis**.

### Algorithm Used

The company applied **K-Means Clustering** to group customers into 4 clusters.
They used the **Silhouette Score** to confirm the best number of clusters.

### Results and Insights

Four main customer groups were identified:

1. **Champions** — buy frequently and spend the most.
2. **Loyal Customers** — buy often but spend moderately.
3. **At-Risk Customers** — used to buy often but have stopped recently.
4. **New Customers** — just joined and made few purchases.

This helped the company create **targeted campaigns**, increasing email response rates by 25%.

---

## 🧾 Summary

* Clustering is **unsupervised learning** used to find hidden groups in unlabeled data.
* Popular algorithms: **K-Means**, **Hierarchical**, and **DBSCAN**.
* Evaluation metrics include **Elbow Method**, **Silhouette Score**, and **Davies–Bouldin Index**.
* Key challenges include choosing *k*, handling outliers, and working with complex data.
* Real-world applications: customer segmentation, image grouping, anomaly detection, and market research.

---

## 📚 References

Smith, J., Brown, A., & Chen, M. (2022). *Enhancing E-Commerce Profitability via RFM and K-Means Segmentation*. Journal of Applied Data Science, 12(4), 112–130.
