# Image Compression with SVD

Singular Value Decomposition (SVD) is a matrix factorization technique used in image compression to reduce the amount of data required to represent an image while preserving important features.

## Mathematical Formulation
Given an image represented as a matrix $A$ (e.g., grayscale pixel values):

$$
A = U \Sigma V^T
$$

- $U$: Left singular vectors
- $\Sigma$: Diagonal matrix of singular values
- $V^T$: Right singular vectors

To compress, keep only the top $k$ singular values and corresponding vectors:

$$
A_k = U_k \Sigma_k V_k^T
$$

## Steps in Image Compression
1. Compute the SVD of the image matrix.
2. Retain only the largest $k$ singular values.
3. Reconstruct the image using the reduced matrices.

## Applications
- Image compression
- Noise reduction
- Latent semantic analysis

SVD allows for efficient storage and transmission of images with minimal loss of quality.
