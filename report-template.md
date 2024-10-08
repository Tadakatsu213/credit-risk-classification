# Module 12 Report Template

## Overview of the Analysis

The purpose of this analysis is to predict the likelihood of loan default based on historical financial data using machine learning. The dataset contains various financial features, and the goal is to predict whether a loan is classified as healthy (0) or high-risk (1).

We focused on predicting the loan_status column, where a value of 0 indicates a healthy loan and a value of 1 indicates a high-risk loan. Using logistic regression, we aimed to predict the loan status based on the features provided in the dataset.

## Stages of the Machine Learning Process:
Data Preparation: The loan_status column was separated as the label (y), and the remaining columns were used as features (X).

Data Splitting: The data was split into training and testing datasets using train_test_split.

Model Training: A Logistic Regression model was trained using the training data.

Model Evaluation: The model’s performance was evaluated through a confusion matrix and a classification report, focusing on accuracy, precision, and recall scores.
## Results

Logistic Regression Model:
Accuracy: 99.27%
Precision: 99.82% (for class 0), 84.54% (for class 1)
Recall: 99.43% (for class 0), 94.51% (for class 1)

## Summary

The logistic regression model performed well, with an overall accuracy of 99.27%. While the model’s precision and recall for predicting healthy loans (class 0) were nearly perfect, its performance for predicting high-risk loans (class 1) showed slightly lower precision but high recall. This means that the model is effective at identifying high-risk loans but may occasionally classify a healthy loan as high-risk.

Given the high recall for high-risk loans, this model can be recommended for predicting credit risk. It balances the need for accurate identification of risky loans while minimizing the risk of false negatives.