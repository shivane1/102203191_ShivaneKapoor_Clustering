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

Results -

![image](https://github.com/user-attachments/assets/2510d219-67d3-4fab-af3c-be93095ad75f)
![image](https://github.com/user-attachments/assets/01e33524-24b0-4a0e-8b33-4b7a56ce800c)
![image](https://github.com/user-attachments/assets/b0f5dd35-b4ef-4505-b148-03d44381b781)
