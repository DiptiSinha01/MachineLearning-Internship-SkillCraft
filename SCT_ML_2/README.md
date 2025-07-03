# 🧠 Customer Segmentation Using K-Means Clustering

A real-world unsupervised learning project to segment customers of a retail store based on their purchase behavior using K-Means Clustering.  
This project was completed as part of a data science internship task.

---

## 📂 Dataset

- **Source:** [Kaggle - Customer Segmentation](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)
- **File Used:** `Mall_Customers.csv`
- **Records:** 200 customers
- **Features:** `CustomerID`, `Gender`, `Age`, `Annual Income (k$)`, `Spending Score (1-100)`

---

## 🎯 Objective

To use K-Means Clustering to group customers into distinct segments based on their spending patterns and income. The goal is to help retail businesses tailor marketing strategies for different customer groups.

---

## 🛠️ Technologies Used

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Scikit-learn
- KMeans, Pipeline, ColumnTransformer, OneHotEncoder, StandardScaler
- Silhouette Score for clustering evaluation

---

## 📊 Approach

### ✅ Baseline Model (2 Features)
- Features: `Annual Income`, `Spending Score`
- Preprocessing: Standard Scaling
- Evaluation: Silhouette Score = **0.555**
- Result: 5 distinct clusters with clear separation

### 🧪 Enhanced Model (4 Features)
- Features: `Gender`, `Age`, `Annual Income`, `Spending Score`
- Preprocessing: OneHotEncoding + Standard Scaling via `Pipeline` and `ColumnTransformer`
- Evaluation: Silhouette Score = **0.3 – 0.5** (depending on `n_clusters`)
- Insight: Adding more features did **not improve** clustering quality due to increased dimensionality and less relevant variables

---

## 🧠 Key Learnings & Insights

- **Silhouette Score** is crucial for evaluating clustering performance
- **Simplicity often wins**: 2D clustering (Income + Spending) gave clearer and more actionable segmentation
- Clusters uncovered segments like:
  - High income, low spenders
  - Average income, high spenders (potential marketing targets)
  - Low income, low spenders
