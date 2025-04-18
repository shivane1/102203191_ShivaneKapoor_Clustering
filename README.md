# 102203191_ShivaneKapoor_Clustering
# Comparitive performance study of different clustering algorithms using different pre-processing techniques with different numbers of clusters on different evaluation parameters
Overview - This project presents a comparative analysis of different clustering algorithms using various preprocessing techniques and cluster numbers, evaluated across several performance metrics. The Iris dataset from the UCI Machine Learning Repository is used as the benchmark. The study aims to highlight how preprocessing and algorithm choice impact clustering quality. Dataset: Iris

Methodology - Preprocessing Techniques No Data Processing: Raw features

Normalization: MinMaxScaler

Transform: StandardScaler

PCA: Principal Component Analysis (2 components)

T+N: StandardScaler after MinMaxScaler

T+N+PCA: PCA after both scaling methods

Clustering Algorithms - K-Means Clustering

Agglomerative (Hierarchical) Clustering

K-Means Shift Clustering

Cluster Numbers - Experiments conducted with c = 3, 4, 5 clusters (where applicable)

Evaluation Metrics - Silhouette Score: Measures cluster cohesion and separation (higher is better)

Calinski-Harabasz Index: Ratio of between-cluster to within-cluster dispersion (higher is better)

Davies-Bouldin Index: Average similarity between clusters (lower is better)

# Results -

![image](https://github.com/user-attachments/assets/2510d219-67d3-4fab-af3c-be93095ad75f)
![image](https://github.com/user-attachments/assets/01e33524-24b0-4a0e-8b33-4b7a56ce800c)
![image](https://github.com/user-attachments/assets/b0f5dd35-b4ef-4505-b148-03d44381b781)




# Findings:

Preprocessing Impact: The choice of preprocessing method had a substantial effect on clustering outcomes. Techniques such as MinMax Scaling and combined scaling pipelines (MinMax → Standard) consistently outperformed raw data, especially in terms of Silhouette and Calinski-Harabasz scores.

K-Means Clustering: This algorithm generally delivered the most reliable performance, especially when the number of clusters was set to 3, which aligns with the actual number of classes in the Iris dataset. It achieved the highest Silhouette and Calinski-Harabasz scores across multiple preprocessing pipelines.

Agglomerative Clustering: The hierarchical clustering method demonstrated high sensitivity to the type of preprocessing applied. In some configurations, especially without proper scaling, it produced unbalanced or overlapping clusters, reflected in poorer evaluation scores.

Mean Shift Clustering: This density-based method automatically determined the number of clusters. It was less affected by preprocessing variations but often failed to detect exactly 3 clusters, which limited its comparability. When 3 clusters were detected, performance was moderate.

Davies-Bouldin Index Observations: This index yielded lowest (best) scores when clusters were well-separated, which most commonly occurred after normalization or PCA-based preprocessing. This reinforces the importance of dimensionality reduction and feature scaling for optimal cluster compactness and separation.
