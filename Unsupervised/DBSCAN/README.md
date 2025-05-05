# DBSCAN

DBSCAN (Density-Based Spatial Clustering of Applications with Noise) is an unsupervised clustering algorithm that groups together points that are closely packed and marks points that lie alone in low-density regions as outliers.

## Algorithm Steps
1. For each point, count the number of points within a radius $\varepsilon$ (epsilon).
2. If the number is at least `min_samples`, the point is a core point and forms a cluster with its neighbors.
3. Expand clusters by recursively including density-reachable points.
4. Points not reachable from any core point are labeled as noise (outliers).

## Key Parameters
- $\varepsilon$ (epsilon): Neighborhood radius
- `min_samples`: Minimum points to form a dense region

## Advantages
- Finds arbitrarily shaped clusters
- Robust to outliers
- No need to specify the number of clusters

## Limitations
- Sensitive to parameter selection
- Struggles with varying density

DBSCAN is widely used for spatial data and anomaly detection.
