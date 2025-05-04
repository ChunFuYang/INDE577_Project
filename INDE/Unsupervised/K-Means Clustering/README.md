# K-Means Clustering

K-Means is an unsupervised clustering algorithm that partitions data into $k$ clusters, where each data point belongs to the cluster with the nearest mean (centroid).

## Algorithm Steps
1. Initialize $k$ cluster centroids randomly.
2. Assign each data point to the nearest centroid.
3. Update centroids by computing the mean of assigned points.
4. Repeat steps 2 and 3 until assignments do not change or a maximum number of iterations is reached.

## Objective Function
K-Means minimizes the within-cluster sum of squares (WCSS):

$$
\text{WCSS} = \sum_{i=1}^k \sum_{x \in C_i} \|x - \mu_i\|^2
$$

- $C_i$: Cluster $i$
- $\mu_i$: Centroid of cluster $i$

## Properties
- Sensitive to initial centroids
- Assumes spherical clusters of similar size

## Applications
- Market segmentation
- Image compression
- Document clustering

K-Means is efficient but may converge to local minima.
