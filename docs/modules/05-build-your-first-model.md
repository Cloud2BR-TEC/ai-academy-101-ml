# 05. Build Your First Model

This module walks through a complete first ML build with clear execution checkpoints.

![Collect data first](../assets/img/collect_data_init_primary_second_targets.svg)

## Step 1: Define Input and Target

- Features: what you give the model.
- Target: what you want the model to predict.

![Feature engineering](../assets/img/feature_engineering_collect_data.svg)

## Step 2: Split Data

Keep some data hidden for evaluation.

- Training set: for learning.
- Test set: for final checking.

![Train test split](../assets/img/training_test_split.svg)

## Step 3: Choose a First Model

Recommended first model options:

- Linear Regression (simple numeric prediction).
- Decision Tree (easy to explain).
- Random Forest (strong baseline for many datasets).

![Decision tree](../assets/img/decision-tree.svg)

![Random forest](../assets/img/random-forest.svg)

## Step 4: Understand Core Metrics

- MAE: average prediction error size.
- MSE: squared errors (penalizes big misses).
- RMSE: error in original unit.
- $R^2$: how much variation model explains.

![Bias variance](../assets/img/bias-variance-tradeoff.svg)

![Gradient descent loss](../assets/img/gradient-descent-loss.svg)

## Step 5: Interpret Results

- If train is great and test is bad -> overfitting.
- If both are weak -> underfitting or poor features.

![Linear regression fit](../assets/img/linear-regression-fit.svg)

## Checklist Before You Continue

- Data cleaned.
- Split verified.
- Metric values recorded.
- Model saved.
