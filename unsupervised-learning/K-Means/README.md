# K-Means Clustering

## What is K-Means?

K-Means is a popular unsupervised machine learning algorithm used for clustering data into distinct groups. The goal of K-Means is to partition a set of data points into **K** clusters, where each point belongs to the cluster with the nearest mean (centroid), resulting in clusters with high intra-group similarity and low inter-group similarity.

## How Does K-Means Work?

The K-Means algorithm operates through the following iterative process:

1. **Initialization**: Choose the number of clusters, K, and randomly select K initial centroids (cluster centers) from the data.
2. **Assignment**: Assign each data point to the nearest centroid, forming K clusters.
3. **Update**: Recalculate the centroids as the mean of all points assigned to each cluster.
4. **Repeat**: Repeat the assignment and update steps until the centroids no longer change significantly or a maximum number of iterations is reached.

This process minimizes the **within-cluster sum of squares (WCSS)**, which is a measure of the variance within each cluster.

### Pseudocode

```
1. Select K initial centroids randomly
2. Repeat until convergence:
    a. Assign each point to the nearest centroid
    b. Recalculate centroids as mean of assigned points
```

<img width="587" height="420" alt="image" src="https://github.com/user-attachments/assets/4f5216a9-02cc-4593-aade-1bd9afdc6dc6" />


## Real-World Applications of K-Means

K-Means clustering is widely used in various domains, including:

- **Image Compression**: Reducing the number of colors in an image by clustering similar pixel colors.
- **Customer Segmentation**: Grouping customers based on purchasing behavior for targeted marketing.
- **Document Clustering**: Organizing documents into topic-based clusters for information retrieval.
- **Anomaly Detection**: Identifying unusual patterns in data, such as fraud detection in banking.
- **Genomics**: Grouping genes with similar expression patterns for biological analysis.
- **Market Basket Analysis**: Discovering groups of products frequently purchased together.

## Summary

K-Means is a simple and efficient algorithm for unsupervised clustering tasks, making it a valuable tool for data exploration and pattern discovery in a wide range of practical applications.
