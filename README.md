# Credit Card Fraud Classifier

A machine learning project for detecting fraudulent credit card transactions, built with scikit-learn.

## Overview

Credit card fraud detection is a highly imbalanced classification problem, fraudulent transactions make up a tiny fraction of all transactions. Only about 0.17% of transactions in this dataset are fraud, so a model that predicts "not fraud" every time would be 99.8% accurate and completely useless. The goal of this project is not just to classify fraudulent transactions, but also to properly evaluate the model's performance.

### Dataset

[mlg-ulb Credit Card Fraud dataset from Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) (~285K transactions, 492 fraud cases, features V1-V28 are PCA-anonymized, Time and Amount are not)

### Process

Starting with Logistic Regression as a baseline, then moving to Random Forest and possibly XGBoost

### Validation

- Evaluating everything with Stratified K-Fold cross-validation
- Handling the class imbalance with class weighting and/or
  - Maybe SMOTE (generating synthetic fraud examples)
