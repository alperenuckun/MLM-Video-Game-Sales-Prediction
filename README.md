# Machine Learning Model Comparison for Video Game Sales Prediction

## Overview
This project aims to predict global sales of video games using machine learning models. We compare multiple regression models and visualize their performance.

## Dataset
The dataset used in this project is vgsales.csv, which contains video game sales data, including:

Platform: The console/platform the game was released on.

Genre: Type of game (e.g., Action, Sports, RPG, etc.).

Sales: Sales numbers in different regions (NA, EU, JP, Other) and global sales.

## Models Implemented
The following regression models are trained and evaluated:

Linear Regression

Ridge Regression

Lasso Regression

K-Nearest Neighbors

Decision Tree Regressor

Extra Tree Regressor

Random Forest Regressor

Bagging Regressor

AdaBoost Regressor

Gradient Boosting Regressor

Support Vector Machine (SVM)

XGBoost Regressor

## Preprocessing Steps

Handling Missing Values:

The Year column is filled with its mean value.

The Publisher column is filled with its most frequent value.

Encoding Categorical Variables:

The Platform and Genre columns are converted to numerical values using Label Encoding.

Feature Selection:

Selected features: Platform, Genre, NA_Sales, EU_Sales, JP_Sales, Other_Sales.

Target variable: Global_Sales.

## Model Evaluation

R² Score: Measures the proportion of variance explained by the model.

Mean Squared Error (MSE): Average squared difference between actual and predicted values.

Mean Absolute Error (MAE): Average absolute difference between actual and predicted values.

Training Time: Time taken to train each model.

## Visualizations

Feature Correlation Heatmap: Displays relationships between numeric features.

Model Performance Analysis:

Bar plot comparing R² Scores of different models.

Boxplot showing the distribution of model performance.

Scatter plot illustrating the relationship between training time and R² Score.

## Usage

Installation

Ensure you have the required dependencies installed:

pip install pandas numpy seaborn matplotlib scikit-learn xgboost

Running the Script

Execute the Python script to train models and generate visualizations:

python model_comparison.py

Expected Output

Printed R² Score, MSE, MAE, and Training Time for each model.

Visualization plots comparing model performances.
