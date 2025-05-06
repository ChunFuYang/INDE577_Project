# The Perceptron

The Perceptron is a foundational algorithm in machine learning for binary classification. It is a type of linear classifier that attempts to find a hyperplane that separates data points of two classes.

## Algorithm Overview
Given input features $x = (x_1, x_2, ..., x_n)$, the Perceptron computes a weighted sum:

$$
z = w_0 + w_1 x_1 + w_2 x_2 + ... + w_n x_n
$$

The output is determined by the sign of $z$:
- If $z \geq 0$, predict class 1
- If $z < 0$, predict class 0

## Learning Rule
The Perceptron updates its weights whenever it misclassifies a sample:

$$
w_j := w_j + \eta (y^{(i)} - \hat{y}^{(i)}) x_j
$$

- $w_j$: Weight for feature $j$
- $\eta$: Learning rate
- $y^{(i)}$: True label
- $\hat{y}^{(i)}$: Predicted label
- $x_j$: Feature value

## Limitations
- Only works for linearly separable data
- Cannot solve problems that are not linearly separable (e.g., XOR problem)

## Applications
- Early neural networks
- Pattern recognition

The Perceptron is the building block for more complex neural networks.

## References
- Rosenblatt, F. (1958). The Perceptron: A Probabilistic Model for Information Storage and Organization in the Brain. Psychological Review, 65(6), 386-408.
- scikit-learn documentation: https://scikit-learn.org/stable/modules/linear_model.html#perceptron
