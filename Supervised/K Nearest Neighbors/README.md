# K Nearest Neighbors (KNN)

K Nearest Neighbors (KNN) is a simple, non-parametric algorithm used for classification and regression. It makes predictions based on the $k$ closest data points in the feature space.

## Algorithm Steps
1. Choose the number of neighbors $k$.
2. Compute the distance (e.g., Euclidean) between the query point and all training samples.
3. Select the $k$ nearest neighbors.
4. For classification: assign the most common class among the neighbors.
5. For regression: average the values of the neighbors.

## Distance Metric
For two points $x$ and $y$ in $n$-dimensional space:

$$
\text{Euclidean distance} = \sqrt{\sum_{i=1}^n (x_i - y_i)^2}
$$

## Properties
- **Lazy learning:** No explicit training phase.
- **Sensitive to feature scaling and irrelevant features.**

## Applications
- Pattern recognition
- Recommendation systems
- Anomaly detection

KNN is easy to implement but can be computationally expensive for large datasets.

## References
- Cover, T., & Hart, P. (1967). Nearest neighbor pattern classification. IEEE Transactions on Information Theory, 13(1), 21-27.
- scikit-learn documentation: https://scikit-learn.org/stable/modules/neighbors.html
