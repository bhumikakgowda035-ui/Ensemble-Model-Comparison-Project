# Performance Comparison Report

## Objective
Compare a baseline Decision Tree with Random Forest and Gradient Boosting classifiers on the same held-out test set.

## Dataset and preprocessing
The notebook loads the Breast Cancer Wisconsin (Diagnostic) dataset from scikit-learn. It checks data types and missing values, separates features and target, and creates stratified training/testing sets. All three models use the same split to make the comparison fair.

## Models
- **Decision Tree:** simple baseline; easy to interpret but can overfit.
- **Random Forest:** combines many decision trees and averages their predictions; generally more robust.
- **Gradient Boosting:** builds trees sequentially to correct earlier errors; can perform well but may require careful tuning.

## Results
Run `notebooks/ensemble_exploration.ipynb` to generate the measured metrics and replace this section with the output saved by the notebook.

## Discussion
Compare accuracy and F1-score, especially because the target classes should both be considered. A deeper decision tree may overfit. Random Forest reduces variance by averaging trees. Gradient Boosting may capture complex patterns but can be sensitive to hyperparameters. The best model is the one with the strongest test-set metrics while keeping the project's limitations in mind.

## Limitations
A single train/test split is only one estimate of generalization. Dataset results do not imply suitability for real clinical use.
