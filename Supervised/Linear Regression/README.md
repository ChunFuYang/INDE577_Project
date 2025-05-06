# Linear Regression

Linear Regression is a fundamental algorithm in statistics and machine learning used to model the relationship between a dependent variable (target) and one or more independent variables (features). The goal is to find the best-fitting straight line (in the case of one feature) or hyperplane (for multiple features) that predicts the target variable.

## Mathematical Formulation
For a single feature (simple linear regression):

$$
y = w_0 + w_1 x + \epsilon
$$

- $y$: Target variable
- $x$: Feature
- $w_0$: Intercept (bias)
- $w_1$: Slope (weight)
- $\epsilon$: Error term

For multiple features (multiple linear regression):

$$
y = w_0 + w_1 x_1 + w_2 x_2 + ... + w_p x_p + \epsilon
$$

## Objective
The algorithm finds the weights ($w$) that minimize the sum of squared errors (residuals) between the predicted and actual values:

$$
\text{MSE} = \frac{1}{n} \sum_{i=1}^n (y_i - \hat{y}_i)^2
$$

where $\hat{y}_i$ is the predicted value for the $i$-th sample.

## Applications
- Predicting house prices
- Forecasting sales
- Estimating trends

Linear Regression assumes a linear relationship, homoscedasticity (constant variance of errors), and independence of errors.

## References
- Freedman, D. A. (2009). Statistical Models: Theory and Practice. Cambridge University Press.
- scikit-learn documentation: https://scikit-learn.org/stable/modules/linear_model.html#linear-regression
