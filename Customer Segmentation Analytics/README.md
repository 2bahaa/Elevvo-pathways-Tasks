# 🛍️ Customer Segmentation Using Clustering (K-Means & DBSCAN)

This project performs **Customer Segmentation** based on customers’ **Annual Income** and **Spending Score** using unsupervised learning techniques like **K-Means** and **DBSCAN**.  
The goal is to identify distinct customer groups to support better business decisions, marketing strategies, and personalized services.

---

## 📁 Dataset

- **Source**: `Mall_Customers.csv` (You can upload your own Excel/CSV file in Colab)
- **Features used**:
  - `Annual Income (k$)`
  - `Spending Score (1-100)`

---

## ⚙️ Techniques Used

### 📊 Data Preprocessing
- Load dataset (CSV or Excel)
- Handle missing values
- Use only two features for clustering: `Annual Income` and `Spending Score`
- Apply feature scaling using `StandardScaler`
- Exploratory Data Analysis (EDA) with scatter plots and distributions

### 📈 Clustering Algorithms
- **K-Means Clustering**
  - Determine optimal number of clusters using:
    - Elbow Method
    - Silhouette Score
  - Final model uses **k = 5**
- **DBSCAN (Density-Based Spatial Clustering)**
  - Explored for noise and arbitrary-shape clusters
  - Tuned parameters: `eps`, `min_samples`

---

## 🔍 Visualizations

- 2D scatter plots of clusters (colored by label)
- Cluster centers for KMeans
- PCA projection (optional)
- Customer distribution per cluster
- Spending and income stats (mean, std, min, max) per cluster

---

## 📈 Evaluation Metrics


Silhouette Score (KMeans, k=5): 0.564
Silhouette Score (DBSCAN):      0.350


## 📊 Sample Cluster Profiling (KMeans) 

| Cluster | Income (mean) | Spending (mean) | Customers | Description                |
|---------|----------------|------------------|-----------|----------------------------|
|   0     | Medium (~54k)  | Medium (~50)     |    79     | Balanced earners/spenders  |
|   1     | High (~84k)    | Low (~19)        |    35     | Rich but low spenders      |
|   2     | Low (~26k)     | Low (~20)        |    22     | Low income, low spending   |
|   3     | High (~84k)    | High (~82)       |    37     | Premium customers 💎       |
|   4     | Low (~26k)     | High (~78)       |    21     | Price-sensitive spenders   |


## 📌 Business Value
Performing customer segmentation helps your business:

🎯 Launch targeted marketing campaigns

🤝 Offer personalized discounts or loyalty programs

💼 Understand customer behavior and value

📈 Prioritize high-value customers

