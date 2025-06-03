# Credit Card Customer Clustering

This project applies unsupervised machine learning techniques—K-Means and Hierarchical Clustering—to analyze and group credit card customers based on their financial behavior.

## Objective
To segment customers using clustering techniques to uncover behavioral patterns, potentially aiding targeted marketing or credit risk analysis.

## Steps Performed

### 1. Data Preparation
- **Loaded Dataset**: `CC General.csv`
- **Handled Missing Values**:
  - Dropped rows with missing `CREDIT_LIMIT`.
  - Filled missing `MINIMUM_PAYMENTS` with the median.
- **Dropped ID Columns**: `CUST_ID` was removed to focus on numerical features.

### 2. Preprocessing
- **Standardization**: Used `StandardScaler` to standardize features.
- **Normalization**: Applied `normalize()` to ensure uniform scaling.
- **Dimensionality Reduction**: Reduced to 2 principal components using PCA for visualization.

### 3. Hierarchical Clustering
- **Algorithm Used**: Agglomerative Clustering with Euclidean distance and complete linkage.
- **Cluster Visualization**: Created scatter plots of the 2D PCA result colored by cluster.
- **Dendrogram**: Visualized hierarchy of clusters to suggest possible number of clusters.

### 4. K-Means Clustering
- **Algorithm Used**: KMeans with 4 clusters.
- **Cluster Labels**: Assigned cluster labels to each data point.
- **Result Visualization**: Not included but recommended as an enhancement.

## Requirements
- pandas
- scikit-learn
- matplotlib
- scipy

