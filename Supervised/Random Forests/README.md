# Random Forests

Random Forests are ensemble learning algorithms that combine multiple decision trees to improve predictive performance and reduce overfitting. They are used for both classification and regression tasks.

## Algorithm Overview
1. **Bootstrap Sampling:** Randomly sample the training data with replacement to create multiple subsets.
2. **Tree Construction:** For each subset, build a decision tree using a random subset of features at each split.
3. **Aggregation:** For classification, use majority voting; for regression, use the average prediction.

## Key Concepts
- **Bagging:** Reduces variance by averaging multiple models trained on different data samples.
- **Feature Randomness:** At each split, a random subset of features is considered, increasing diversity among trees.

## Advantages
- High accuracy
- Robust to overfitting
- Handles large datasets and high-dimensional spaces

## Limitations
- Less interpretable than single decision trees
- Can be computationally intensive

Random Forests are widely used for their strong performance and versatility.

## References
- Breiman, L. (2001). Random Forests. Machine Learning, 45(1), 5-32.
- scikit-learn documentation: https://scikit-learn.org/stable/modules/ensemble.html#random-forests
