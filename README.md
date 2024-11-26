# Student Performance Analysis and Prediction

## Overview
This project analyzes the student performance dataset and develops a predictive model for the final grade (`G3`). The analysis involves feature engineering, visualization, and model evaluation. The goal is to understand factors influencing student performance and build a robust predictive model.

## Dataset
The analysis is based on the [Student Performance Dataset](https://archive.ics.uci.edu/ml/datasets/Student+Performance). The dataset includes attributes such as:
- **Demographics**: Age, gender, address type, etc.
- **Academic Information**: Previous grades (`G1`, `G2`), study time, failures.
- **Parental and Social Information**: Parent education levels, family support, relationships.

## Key Features

### Exploratory Data Analysis
- Visualized the correlation between features using heatmaps.
- Highlighted significant features such as `G2` (second-period grade), `G1` (first-period grade), and absences.

### Predictive Modeling
- Built an **XGBoost Regressor** to predict `G3`.
- Evaluated the model with metrics such as MAE (Mean Absolute Error) and R² score.

### Insights from Feature Importance
- The model heavily relies on `G2`, followed by `absences`.
- Certain features, such as `famsup` and `activities`, showed minimal impact.

### Error Analysis
- Examined erroneous predictions, highlighting commonalities among misclassified samples.
- Observed that students with `G3 = 0` but non-zero `G1` and `G2` tend to confuse the model, likely indicating missing exams.

### Future Work
- Introduce a binary column indicating whether `G3 = 0`.
- Transform `G3` to be the average of `G1` and `G2`.
- Explore alternative models better suited to handling outliers.

## Visualizations
The notebook includes:
1. Heatmaps for feature correlations.
2. Bar plots showing feature importance.
3. Line plots for grade distributions (`G1`, `G2`, `G3`).
4. Comparison of feature distributions for best, worst, and overall predictions.

### Prerequisites
- Python 3.7+
- Required Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `xgboost`, `scikit-learn`


