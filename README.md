# Customer-Segmentation
This project applies K-Means clustering to the Mall Customer Segmentation dataset (Kaggle). Customers are grouped by age, annual income, and spending score. The optimal number of clusters was determined using three independent metrics, and each cluster was profiled to extract actionable business insights.

How It Works

EDA — Distribution plots, scatter plots, and correlation heatmap
Feature Selection — Age, Annual Income, Spending Score
Standardization — StandardScaler (mean=0, std=1) for fair distance calculations
Optimal k Selection — Elbow Method (WCSS), Silhouette Score, Calinski-Harabasz Index → k=6
K-Means Clustering — Applied with 25 initializations for stability
Cluster Profiling — Mean values per cluster to interpret each customer group


How to Run
bashgit clone https://github.com/Khalfani04/customer-segmentation-kmeans
cd customer-segmentation-kmeans
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook COSC32000_Assignment1_KMeans.ipynb

Results
Metric -> Optimal k
Elbow Method (WCSS) -> 5
Silhouette Score -> 6
Calinski-Harabasz Index -> 6
Final Choice ->6
6 distinct customer segments identified, ranging from high-income/high-spend to low-income/low-spend groups.

What I Learned:
How to select the right number of clusters using multiple validation metrics
Why feature standardization is essential before distance-based algorithms
How to translate cluster profiles into business-readable insights
