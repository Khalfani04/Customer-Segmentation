# 🛍️ Customer Segmentation — K-Means Clustering

> Segments mall customers into behavioural groups using unsupervised machine learning to support data-driven business decisions.

---

## Overview

This project applies K-Means clustering to the Mall Customer Segmentation dataset (Kaggle). Customers are grouped by age, annual income, and spending score. The optimal number of clusters was determined using three independent metrics, and each cluster was profiled to extract actionable business insights.

**Dataset:** [Mall Customer Segmentation Data — Kaggle](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)

---

## Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=flat-square)

---

## How It Works

1. **EDA** — Distribution plots, scatter plots, and correlation heatmap
2. **Feature Selection** — Age, Annual Income, Spending Score
3. **Standardization** — StandardScaler (mean=0, std=1) for fair distance calculations
4. **Optimal k Selection** — Elbow Method (WCSS), Silhouette Score, Calinski-Harabasz Index → k=6
5. **K-Means Clustering** — Applied with 25 initializations for stability
6. **Cluster Profiling** — Mean values per cluster to interpret each customer group

---

## How to Run

```bash
git clone https://github.com/Khalfani04/customer-segmentation-kmeans
cd customer-segmentation-kmeans
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook COSC32000_Assignment1_KMeans.ipynb
```

---

## Results

| Metric | Optimal k |
|--------|-----------|
| Elbow Method (WCSS) | 5 |
| Silhouette Score | 6 |
| Calinski-Harabasz Index | 6 |
| **Final Choice** | **6** |

6 distinct customer segments identified, ranging from high-income/high-spend to low-income/low-spend groups.

---

## What I Learned

- How to select the right number of clusters using multiple validation metrics
- Why feature standardization is essential before distance-based algorithms
- How to translate cluster profiles into business-readable insights

---

## Contact

**Khalfani Norman** · [LinkedIn](https://www.linkedin.com/in/YOUR-LINKEDIN) · [GitHub](https://github.com/Khalfani04)
