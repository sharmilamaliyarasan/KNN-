# 🏠 House Price Prediction Using k-NN Regression

## 📋 Project Overview

This project predicts house prices using k-Nearest Neighbors (k-NN) regression, a distance-based, non-parametric algorithm:

k-NN predicts a house price by averaging the prices of the k most similar houses in the feature space.

Unlike linear regression, k-NN does not assume any functional form between features and target.

Key steps include feature scaling, cross-validation to select k, training, and evaluation on a test set.

## 🗂 Dataset Details

Input Features:

size_sqft — House area in square feet

bedrooms — Number of bedrooms

bathrooms — Number of bathrooms

age — House age in years

distance_city_center_km — Distance from city center

Target Variable:

price — House price

Purpose:

Predict house prices accurately using k-NN regression

Analyze which features impact prediction errors

## 📊 Visualization

Predicted vs Actual Prices

Scatter plot of predicted vs actual house prices

<img width="567" height="453" alt="image" src="https://github.com/user-attachments/assets/17cfdb8b-c90a-401a-9f7c-1b9e5617d860" />


Red dashed line represents perfect predictions

Scatter plots of prediction errors against each feature

Helps identify which features cause larger errors

## 🔍 Insights & Notes

k-NN Regression:

Sensitive to feature scaling → StandardScaler used

Best k selection via 5-fold cross-validation → Ensures optimal prediction

No coefficients → Feature importance is inferred via error analysis

Feature Impact Analysis:

Errors vs features show where the model struggles

Features with systematic error patterns may need transformations

Model Performance (example metrics):

Best k: 5

Test RMSE: 34,500 (example)

Test R²: 0.82 (example)

Strengths:

Simple and intuitive

Captures non-linear relationships between features and price

Limitations:

Sensitive to outliers and irrelevant features

Performance depends on choice of k and feature scaling

Does not provide direct feature importance

## ✅ Conclusion

k-NN regression provides a flexible, non-parametric approach to predict house prices.

Cross-validation helps choose the best k for minimizing errors.

Feature-error analysis offers insights into which features influence prediction accuracy.

Best suited for datasets where relationships between features and target are non-linear or unknown.
