# Logistic Regression

Logistic Regression is a statistical algorithm used for binary classification. It models the probability that a given input belongs to a particular class using the logistic (sigmoid) function.

## Mathematical Formulation
Given input features $x = (x_1, x_2, ..., x_n)$, the model computes:

$$
z = w_0 + w_1 x_1 + w_2 x_2 + ... + w_n x_n
$$

The probability of class 1 is:

$$
P(y=1|x) = \sigma(z) = \frac{1}{1 + e^{-z}}
$$

- $\sigma(z)$: Sigmoid function
- $w_i$: Weights
- $x_i$: Features

## Objective
The algorithm finds weights that maximize the likelihood of the observed data (maximum likelihood estimation), often by minimizing the binary cross-entropy loss.

## Applications
- Medical diagnosis
- Spam detection
- Credit scoring

Logistic Regression is simple, interpretable, and effective for linearly separable data.
