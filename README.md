# Task 8: Clustering with K-Means

## Objective
The goal of this task is to apply unsupervised learning using the K-Means clustering algorithm to identify meaningful groupings within a dataset. The Mall Customer Segmentation Dataset is used for this purpose.

## Tools and Libraries
- Scikit-learn  
- Pandas  
- Matplotlib  
- StandardScaler (for feature scaling)  
- PCA (for dimensionality reduction)  
- Silhouette Score (for clustering evaluation)

## Steps Followed

### 1. Data Loading and Preparation
The Mall Customer Segmentation dataset was loaded, and the relevant features such as Annual Income and Spending Score were selected for clustering. These features represent customer spending behavior and income levels, making them ideal for segmentation.

### 2. Feature Scaling
StandardScaler was applied to normalize the feature values. This ensures that all features contribute equally to the distance metrics used by K-Means.

### 3. Dimensionality Reduction (Optional)
Principal Component Analysis (PCA) was applied to reduce the feature space to two dimensions for visualization. Although the selected dataset already had two features, PCA ensures robust visualization in cases of higher dimensions.

### 4. Finding Optimal K Using Elbow Method
To determine the best number of clusters (K), the Elbow Method was used. A range of K values was tested, and the corresponding inertia (within-cluster sum of squares) was plotted. The "elbow point" in the plot helped identify the optimal number of clusters.

### 5. Applying K-Means Clustering
K-Means clustering was applied to the standardized data using the optimal number of clusters. Each data point was assigned a cluster label based on its proximity to the centroids.

### 6. Cluster Visualization
The clustering result was visualized in two dimensions using the PCA-reduced data. Each cluster was color-coded, providing an intuitive view of the segmentation results.

### 7. Clustering Evaluation
The quality of the clustering was assessed using the Silhouette Score, which quantifies how well each data point fits into its assigned cluster versus other clusters. A higher score indicates better-defined clusters.

## Conclusion
This task demonstrated the application of K-Means clustering on a real-world customer segmentation dataset. It covered essential unsupervised learning steps, including data preprocessing, model fitting, optimal cluster selection, visualization, and evaluation using Silhouette Score.
