Customer Segmentation Using KMeans Clustering :
Overview
This project focuses on customer segmentation using KMeans clustering on a dataset of mall customers. The goal is to classify customers into different groups based on their purchasing behaviors. This segmentation can help businesses tailor their marketing strategies more effectively to meet the needs of different customer segments.
Dataset
The dataset used is Mall_Customers.csv, which contains the following columns:
CustomerID: Unique ID for each customer
Gender: Gender of the customer
Age: Age of the customer
Annual Income (k$): Annual income of the customer in thousands of dollars
Spending Score (1-100): Spending score assigned to the customer based on their behavior and spending nature
Data Preprocessing
Handling Missing Values: The dataset contains no missing values.
Dropping Irrelevant Columns: The CustomerID column was dropped as it is not needed for clustering.
Encoding Categorical Variables: The Gender column was dropped for simplicity.
Feature Scaling: The Annual Income (k$) and Spending Score (1-100) columns were scaled using MinMaxScaler.
Clustering:
Initial Clustering Attempt
We started by performing KMeans clustering with an arbitrary number of clusters (n_clusters=4). The Gender column was dropped, and the features Annual Income (k$) and Spending Score (1-100) were scaled. The clustering was done on the features Age, Annual Income (k$), and Spending Score (1-100).
Finding the Optimal Number of Clusters:
To determine the optimal number of clusters, we used the Elbow Method. We calculated the Within-Cluster Sum of Squares (WCSS) for different numbers of clusters and plotted the results.
Silhouette Analysis:
Silhouette analysis was used to evaluate the quality of clustering. The silhouette score indicates how well each object lies within its cluster.
Results:
Optimal Clusters: Based on the silhouette scores and the Elbow Method, the optimal number of clusters is determined to be 4.
Cluster Visualization: We visualized the clusters using scatter plots, showing clear segmentation of customers based on their age, annual income, and spending score.
Conclusion:
This project demonstrates the process of customer segmentation using KMeans clustering. By identifying distinct groups within the customer base, businesses can tailor their marketing strategies more effectively to meet the needs of different customer segments.

