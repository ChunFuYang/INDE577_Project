# Gradient Boosting

Gradient Boosting is a supervised ensemble learning method used for both regression and classification. It builds a strong model by sequentially adding weak learners (typically decision trees), where each new learner focuses on correcting the errors of the previous ensemble.

## Algorithm Overview
- **Initialization:** Start with a simple model (e.g., mean of targets for regression).
- **Boosting Rounds:** For each iteration:
  - Compute the residuals (errors) of the current model.
  - Fit a weak learner to these residuals.
  - Update the model by adding the new learner, weighted by an optimal step size.
- **Final Model:** The sum of all learners forms the final prediction.

## Key Formulas
- **Model Update:** \
$F_{m}(x) = F_{m-1}(x) + \gamma_m h_m(x)$ \
  where $F_{m}(x)$ is the model at iteration $m$, $h_m(x)$ is the new weak learner, and $\gamma_m$ is the step size (learning rate).

- **Residuals (for regression):** \
$r_{im} = y_i - F_{m-1}(x_i)$ \
  where $y_i$ is the true value and $F_{m-1}(x_i)$ is the prediction from the previous model.

- **General Loss Minimization:**
  At each step, the new learner $h_m(x)$ is fit to minimize the loss function $L$:\
$h_m(x) = \arg\min_h \sum_{i=1}^n L\left(y_i, F_{m-1}(x_i) + h(x_i)\right)$

## Advantages
- High predictive accuracy
- Works for both regression and classification
- Can handle various loss functions

## Limitations
- Sensitive to overfitting if not properly regularized
- Can be computationally intensive
- Requires careful tuning of parameters

Gradient Boosting is the foundation for popular algorithms like XGBoost, LightGBM, and CatBoost.

## References
- Friedman, J. H. (2001). Greedy Function Approximation: A Gradient Boosting Machine. Annals of Statistics, 29(5), 1189-1232.
- scikit-learn documentation: https://scikit-learn.org/stable/modules/ensemble.html#gradient-boosting
