# Churn Prediction Project

This project focuses on predicting customer churn for a video streaming service using advanced machine learning techniques. The objective is to identify customers at risk of cancelling their subscription, enabling proactive retention strategies.

## Overview
Customer churn prediction is a critical task for subscription-based services. By analyzing user behavior and service usage patterns, we aim to build predictive models that accurately estimate the likelihood of a customer churning in the near future.

## Dataset
The dataset includes anonymized information on user preferences, subscription types, streaming habits, support tickets, and more. It is split into:
- `train.csv`: Training set with features and churn labels
- `test.csv`: Test set for generating predictions
- `data_descriptions.csv`: Column descriptions for all variables

## Features Used
Key features include:
- Monthly charges
- Subscription type
- Payment method
- Viewing hours per week
- Average viewing duration
- Number of support tickets
- Content type preferences

## Modeling Approach
Three models were implemented and evaluated:

### 1. Logistic Regression
- **ROC AUC:** 0.75
- **Highlights:** Simple, interpretable baseline model
- **Strengths:** High recall for churn class; provides clear coefficients for feature importance

### 2. Random Forest Classifier
- **ROC AUC:** 0.74
- **Highlights:** Captures nonlinear relationships and feature interactions
- **Strengths:** Good recall for churn, robust to overfitting

### 3. XGBoost Classifier
- **ROC AUC:** 0.79
- **Highlights:** Best overall model
- **Strengths:** Superior balance between precision and recall, effective with unbalanced data

## Evaluation Metrics
Models were assessed using:
- **Precision, Recall, F1-Score** (per class)
- **ROC AUC Score** (overall)
- **Confusion Matrix** (internal validation)

## Final Output
A submission file `prediction_submission.csv` was created, containing the predicted churn probabilities for each customer in the test set.

## Business Impact
Identifying high-risk customers allows targeted interventions like personalized offers, improving retention and reducing churn-related losses.

## Next Steps
- Perform hyperparameter tuning with cross-validation
- Explore SHAP for model explainability
- Integrate with a dashboard for business stakeholders

---
*Developed as part of the Coursera Data Science Capstone Project.*

