# Decision Trees

Decision Trees are supervised learning algorithms used for classification and regression. They model decisions as a tree-like structure, where each internal node represents a test on a feature, each branch represents an outcome, and each leaf node represents a prediction.

## Algorithm Overview
- **Splitting:** At each node, the data is split based on a feature that maximizes a criterion (e.g., information gain, Gini impurity).
- **Recursion:** The process repeats recursively for each child node.
- **Stopping:** The tree grows until a stopping condition is met (e.g., maximum depth, minimum samples per leaf).

## Splitting Criteria
- **Gini Impurity (for classification):** \
$$
G = 1 - \sum_{i=1}^C p_i^2
$$ \
  where $p_i$ is the proportion of class $i$ samples.
- **Information Gain (Entropy):**
$$
H = -\sum_{i=1}^C p_i \log_2 p_i
$$

## Advantages
- Easy to interpret
- Handles both numerical and categorical data

## Limitations
- Prone to overfitting
- Unstable to small data variations

Decision Trees are the basis for more advanced ensemble methods like Random Forests.

## References
- Breiman, L., Friedman, J. H., Olshen, R. A., & Stone, C. J. (1984). Classification and Regression Trees. Wadsworth.
- scikit-learn documentation: https://scikit-learn.org/stable/modules/tree.html
