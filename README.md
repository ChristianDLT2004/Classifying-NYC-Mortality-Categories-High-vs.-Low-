# Classifying NYC Mortality Categories (High vs. Low)

## Overview
This project develops an end-to-end machine learning pipeline to classify New York City's leading causes of death into **high-mortality** and **low-mortality** categories using demographic and cause-of-death features.

The goal is to explore whether mortality patterns can be reliably predicted from structured public health data and to evaluate the performance of multiple statistical and machine learning models.

## Dataset
- **Source:** NYC Department of Health & Mental Hygiene  
- **Dataset:** New York City Leading Causes of Death  
- Features include year, sex, race/ethnicity, leading cause of death, and mortality rate statistics.

## Methodology
- Cleaned and standardized raw data by handling non-standard missing values and converting numeric fields
- Defined a binary target variable using the median **Age-Adjusted Death Rate**
- Mitigated data leakage by removing highly correlated mortality measures
- Performed exploratory data analysis (EDA) and feature selection using:
  - Chi-square tests
  - Pearson correlation
  - Recursive Feature Elimination (RFE)
- Trained and evaluated multiple models with stratified cross-validation:
  - Logistic Regression
  - Support Vector Machines (SVM)
  - K-Nearest Neighbors (KNN)
  - Decision Trees
  - Ensemble methods (soft voting, Random Forest)

## Evaluation
Models were evaluated using:
- Accuracy
- Precision / Recall / F1-score
- ROC-AUC

Ensemble approaches achieved the strongest overall performance, demonstrating high predictive accuracy and robustness across validation folds.

## Technologies
- Python
- Pandas, NumPy
- scikit-learn
- Matplotlib, Seaborn

## Notes
This project emphasizes **data preprocessing, feature engineering, model evaluation, and responsible handling of correlated variables**, reflecting real-world machine learning workflows in public health analytics.
