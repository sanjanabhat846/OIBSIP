# Task 4 — Email / SMS Spam Detection

## Overview

This project develops a machine learning system for classifying text messages as either spam or legitimate ham messages.

Natural Language Processing (NLP) techniques are used to convert text into numerical features using TF-IDF, followed by machine learning classification.

## Objective

The objective is to identify unwanted spam messages while correctly preserving legitimate messages.

## Dataset

The project uses the SMS Spam Collection Dataset.

The dataset contains two classes:

- `ham` — legitimate messages
- `spam` — unwanted messages

## Workflow

1. Data loading
2. Data cleaning
3. Removal of unnecessary columns
4. Duplicate removal
5. Text preprocessing
6. Label encoding
7. Train-test splitting
8. TF-IDF feature extraction
9. Multinomial Naive Bayes
10. Logistic Regression
11. Model evaluation
12. Confusion matrix analysis
13. Spam word analysis
14. New-message prediction

## NLP Technique

### TF-IDF

TF-IDF (Term Frequency-Inverse Document Frequency) converts text messages into numerical feature vectors that can be processed by machine learning algorithms.

Unigrams and bigrams were used to capture both individual words and two-word combinations.

## Models

### Multinomial Naive Bayes

Multinomial Naive Bayes was used as the primary text classification model.

### Logistic Regression

Logistic Regression was used as an alternative classifier for comparison.

## Results

| Model | Accuracy | Precision | Recall | F1 Score |
|---|---:|---:|---:|---:|
| Multinomial Naive Bayes | 96.32% | 100.00% | 70.99% | 83.04% |
| Logistic Regression | 95.16% | 98.80% | 62.60% | 76.64% |

### Best Model

**Multinomial Naive Bayes** achieved the highest F1 score of **83.04%** and was selected as the best-performing model.

## Why Recall Matters

Recall is particularly important in spam detection because false negatives represent actual spam messages that are incorrectly classified as legitimate messages.

A missed spam message may contain unwanted advertising, phishing attempts, fraudulent offers, or malicious links.

The model achieved a spam recall of approximately **70.99%**, meaning it identified about 71% of the actual spam messages in the test set.

Precision must also be considered because incorrectly classifying legitimate messages as spam can cause important messages to be lost.

## Example Predictions

The trained system successfully classified example messages:

- A normal meeting message → **HAM**
- A prize/reward message → **SPAM**

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- WordCloud
- Jupyter Notebook

## Project Structure

```text
DataScience-Task4-EmailSpamDetection/
│
├── README.md
├── Task4_Email_Spam_Detection.ipynb
└── spam.csv