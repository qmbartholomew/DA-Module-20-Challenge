# DA-Module-20-Challenge - Credit Risk Analysis with Logistic Regression

## Overview

The purpose of this analysis is to evaluate the creditworthiness of loan applicants using machine learning. We used logistic regression to classify loans as either **healthy (0)** or **high-risk (1)** based on applicant data. This analysis can help financial institutions make more informed lending decisions by identifying patterns in the risk profile of applicants.

---

## Results

The logistic regression model was trained on historical lending data and evaluated on a test dataset. Below are the key performance metrics:

- **Accuracy:** High for overall predictions due to dataset imbalance
- **Precision (Healthy Loans - Class 0):** High – the model is good at correctly identifying healthy loans
- **Recall (Healthy Loans - Class 0):** High – few healthy loans are misclassified
- **Precision (High-Risk Loans - Class 1):** Low – the model has difficulty identifying true high-risk cases
- **Recall (High-Risk Loans - Class 1):** Very low – many high-risk loans are misclassified as healthy

---

## Summary

The logistic regression model shows strong performance in predicting healthy loans but struggles significantly with high-risk loans, likely due to class imbalance in the dataset. While it can be used for preliminary screening, **this model should not be used in isolation** for making lending decisions. To improve high-risk loan detection, we recommend:

- Rebalancing the dataset using techniques like oversampling (e.g., SMOTE) or undersampling
- Trying alternative models (e.g., Random Forest, XGBoost)
- Including additional features to improve model signal

Given its limited ability to identify high-risk borrowers, **we do not recommend deploying this model for production use without further enhancements.**

### By Quentin Bartholomew