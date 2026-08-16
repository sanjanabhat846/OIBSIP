# Task 5 — Sales Prediction Using Python

## Overview

This project develops a machine learning regression system to predict sales based on advertising expenditure across TV, Radio, and Newspaper channels.

The project focuses on analyzing the relationship between advertising investment and sales and comparing different regression models.

## Objective

The objective of this project is to:

- Analyze advertising expenditure and sales
- Explore relationships between advertising channels and sales
- Build regression models to predict sales
- Compare model performance using regression metrics
- Identify the most influential advertising channel

## Dataset

The project uses an Advertising Budget and Sales dataset containing **200 observations**.

### Features

- TV Ad Budget ($)
- Radio Ad Budget ($)
- Newspaper Ad Budget ($)

### Target Variable

- Sales ($)

The dataset was cleaned by removing the unnecessary index column and renaming the remaining columns for easier analysis.

## Exploratory Data Analysis

The following analyses and visualizations were performed:

- Dataset inspection
- Descriptive statistics
- Sales distribution
- Pairplot
- TV Advertising vs Sales scatter plot
- Radio Advertising vs Sales scatter plot
- Newspaper Advertising vs Sales scatter plot
- Correlation heatmap

These visualizations were used to understand the relationships between advertising expenditure and sales.

## Machine Learning Models

### 1. Linear Regression

Linear Regression was used as the baseline regression model.

### 2. Random Forest Regression

Random Forest Regression was used as a second regression model to capture potentially nonlinear relationships between advertising expenditure and sales.

## Evaluation Metrics

The models were evaluated using:

- **Mean Absolute Error (MAE)**
- **Root Mean Squared Error (RMSE)**
- **R² Score**

For MAE and RMSE, lower values indicate better performance.

For R² Score, a higher value indicates better model performance.

## Model Results

| Model | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| Linear Regression | — | — | — |
| **Random Forest** | **0.6289** | **0.7577** | **0.9818** |

### Best Performing Model

**Random Forest Regression** was the best-performing model based on R² Score.

The model achieved:

- **MAE:** 0.6289
- **RMSE:** 0.7577
- **R² Score:** 0.9818

The R² score of **0.9818** indicates that the model explains approximately **98.18% of the variation in sales** on the test set.

## Actual vs Predicted Sales

An actual-versus-predicted plot was created to evaluate how closely the model's predictions followed the actual sales values.

Points closer to the diagonal reference line indicate more accurate predictions.

## Residual Analysis

A residual plot was created to examine the prediction errors of the selected model.

Residual analysis helps determine whether the model errors are reasonably distributed around zero and whether there are visible patterns in the errors.

## Feature Importance

Random Forest feature importance was used to analyze the relative predictive importance of the three advertising channels:

- TV
- Radio
- Newspaper

The feature-importance visualization is included in the notebook.

## Sample Prediction

The trained model was used to predict sales for the following hypothetical advertising budget:

| Advertising Channel | Budget |
|---|---:|
| TV | $200 |
| Radio | $40 |
| Newspaper | $30 |

### Predicted Sales

**20.4**

This demonstrates how the trained model can be used to estimate sales for a given advertising budget.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow

```text
Dataset
   ↓
Data Cleaning
   ↓
Exploratory Data Analysis
   ↓
Visualization
   ↓
Train/Test Split
   ↓
Linear Regression
   ↓
Random Forest Regression
   ↓
Model Evaluation
   ↓
Model Comparison
   ↓
Residual Analysis
   ↓
Feature Importance
   ↓
Sales Prediction