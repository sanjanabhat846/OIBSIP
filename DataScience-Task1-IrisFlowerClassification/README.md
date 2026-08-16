# Task 1 — Iris Flower Classification

## Overview

This project builds a machine learning classification system to identify iris flower species based on their physical measurements.

The three target species are:

- Setosa
- Versicolor
- Virginica

## Dataset

The Iris dataset contains 150 flower samples with four numerical features:

- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

## Objectives

- Explore and understand the dataset
- Analyze feature distributions
- Visualize relationships between features and species
- Train classification models
- Evaluate model performance
- Compare different classifiers
- Identify the most discriminative features

## Analysis Performed

- Exploratory Data Analysis
- Data type and missing-value checks
- Class distribution analysis
- Pairplot visualization
- Box plot analysis
- Train-test split
- Logistic Regression
- Decision Tree Classifier
- Accuracy evaluation
- Confusion matrix
- Precision
- Recall
- F1-score
- Model comparison
- Feature importance analysis

## Models Used

### Logistic Regression

Used as a classification baseline for predicting the three iris species.

### Decision Tree Classifier

Used as a second classification approach and to analyze feature importance.

## Results

Logistic Regression was selected as the best-performing model based on the evaluation results.

It achieved an F1-score of approximately **0.9666**.

Feature importance analysis showed that **petal length** and **petal width** were the most discriminative features in the Decision Tree model.

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
DataScience-Task1-IrisFlowerClassification/
│
├── README.md
├── .gitignore
└── Task1_Iris_Flower_Classification.ipynb