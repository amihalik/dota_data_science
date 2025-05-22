# EDA Summary

This document highlights notable patterns from the exploratory data analysis notebook.

## Key Findings
- **Class Imbalance:** The target variable `radiant_win` is slightly imbalanced, so model evaluation should use stratified sampling or class weights.
- **Highly Correlated Features:** Several numeric variables exhibit strong correlations (>0.8). Dimensionality reduction or feature selection may help avoid multicollinearity.
- **Skewed Distributions:** Many features are right-skewed. Applying log or Box-Cox transformations could stabilize variance.
- **Presence of Outliers:** Extreme values in duration and kill counts suggest capping or transformation to reduce their influence.
- **Duration Relationship:** Match duration shows a clear relationship with the outcome, indicating that engineered temporal features may boost performance.

See `notebooks/02_eda.ipynb` for code and generated plots saved under the `figures/` directory.
