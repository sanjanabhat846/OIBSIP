# Task 3 — Car Price Prediction

## Overview

This project develops a machine learning regression system to predict used car sale prices.

The project covers data cleaning, exploratory data analysis, feature engineering, preprocessing, regression model training, evaluation, and feature importance analysis.

## Dataset

The dataset contains used-car listings with information including:

- Manufacturing year
- Fuel type
- Kilometres driven
- City
- Body type
- Transmission
- Make
- Model
- Number of owners
- Original price
- Car rating
- Vehicle certification information
- Sale price

## Objective

The objective is to predict the `sale_price` of a used car using relevant vehicle and listing characteristics.

## Workflow

1. Data loading
2. Dataset inspection
3. Missing-value analysis
4. Duplicate removal
5. Exploratory data analysis
6. Feature engineering
7. Feature selection
8. Train-test split
9. Numerical preprocessing
10. Categorical encoding
11. Linear Regression
12. Random Forest Regression
13. Model evaluation
14. Feature importance analysis
15. Actual vs predicted price analysis

## Feature Engineering

A `car_age` feature was created from the manufacturing year:

`car_age = 2026 - yr_mfr`

## Models Used

### Linear Regression

Used as the baseline regression model.

### Random Forest Regression

Used to capture nonlinear relationships between vehicle characteristics and sale price.

## Results

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Linear Regression | 55,361.75 | 109,394.75 | 0.8673 |
| Random Forest | 38,745.05 | 85,139.22 | 0.9196 |

Random Forest was the best-performing model.

## Feature Importance

The most influential feature was `original_price`, with approximately **55.68%** feature importance.

Other important features included:

- `car_age`
- `yr_mfr`
- Body type
- `kms_run`
- Selected vehicle models and makes

## Evaluation Metrics

### MAE
Mean Absolute Error measures the average absolute difference between actual and predicted prices. Lower values indicate better performance.

### RMSE
Root Mean Squared Error penalizes larger prediction errors more strongly. Lower values indicate better performance.

### R²
R² measures how much variation in the target variable is explained by the model. Higher values indicate better performance.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Structure

```text
DataScience-Task3-CarPricePrediction/
│
├── README.md
├── Task3_Car_Price_Prediction.ipynb
└── Used_Car_Price_Prediction.csv