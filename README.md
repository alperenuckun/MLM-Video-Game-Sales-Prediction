# Machine Learning Model Comparison

## Overview
This project predicts global sales of video games using various machine learning models and compares their performance.

## Dataset
The dataset contains the following features:
- **Platform**: Gaming platform (e.g., PS4, Xbox, etc.)
- **Genre**: Game genre (e.g., Action, Sports, etc.)
- **Sales**: Regional and global sales figures:
  - **NA_Sales**: North America sales
  - **EU_Sales**: Europe sales
  - **JP_Sales**: Japan sales
  - **Other_Sales**: Sales from other regions
  - **Global_Sales**: Total worldwide sales

**Source**: `vgsales.csv`

## Models Used
This project utilizes the following machine learning models:
- **Regression Models**:
  - Linear Regression
  - Ridge Regression
  - Lasso Regression
  - K-Nearest Neighbors (KNN)
- **Tree-Based Models**:
  - Decision Tree
  - Random Forest
  - Extra Trees
- **Ensemble Learning**:
  - Bagging
  - AdaBoost
  - Gradient Boosting
  - XGBoost
- **Support Vector Machine (SVM)**

## Preprocessing
The dataset undergoes the following preprocessing steps:
- **Handling Missing Values**:
  - `Year` → Filled with mean value
  - `Publisher` → Filled with mode value
- **Encoding**:
  - Label Encoding applied to `Platform` and `Genre`
- **Feature Selection**:
  - Input Features: `NA_Sales`, `EU_Sales`, `JP_Sales`, `Other_Sales`
  - Target Variable: `Global_Sales`

## Evaluation Metrics
The models are evaluated based on the following metrics:
- **R² Score** (Coefficient of determination)
- **Mean Squared Error (MSE)**
- **Mean Absolute Error (MAE)**
- **Training Time**

## Visualizations
To analyze the results, the following visualizations are included:
- **Feature Correlation Heatmap**
- **Performance Comparisons**:
  - Bar Plot (R² Score comparison)
  - Box Plot (Error distributions)
  - Scatter Plot (Predicted vs. Actual values)

## Installation & Usage
### Install Dependencies
```sh
pip install pandas numpy seaborn matplotlib scikit-learn xgboost
```
### Run the Model Comparison Script
```sh
python model_comparison.py
```

