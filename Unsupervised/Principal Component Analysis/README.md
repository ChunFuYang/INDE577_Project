# Principal Component Analysis (PCA)

Principal Component Analysis (PCA) is an unsupervised dimensionality reduction technique that transforms data into a new coordinate system, maximizing variance along the axes (principal components).

## Algorithm Steps
1. Standardize the data.
2. Compute the covariance matrix.
3. Calculate eigenvalues and eigenvectors of the covariance matrix.
4. Sort eigenvectors by decreasing eigenvalues and select the top $k$ components.
5. Project the data onto the selected components.

## Mathematical Formulation
Given a data matrix $X$ (centered):
- Covariance matrix: $C = \frac{1}{n-1} X^T X$
- Eigen decomposition: $C v = \lambda v$

## Applications
- Data visualization
- Noise reduction
- Feature extraction

PCA helps to reduce complexity while retaining most of the data's variability.
