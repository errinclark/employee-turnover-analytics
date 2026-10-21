# Employee Turnover Analytics

### Machine Learning Portfolio Project

A machine-learning project exploring employee attrition through exploratory data analysis, clustering, supervised classification, and risk stratification.

## Project Overview

The project examines whether employee data can be used to identify patterns associated with turnover and predict employees at greater risk of leaving. The analysis emphasizes translating predictive results into interpretable information for organizational decision support.

## Methods

- Exploratory data analysis and visualization
- Data cleaning, encoding, and class-imbalance handling using SMOTE
- K-Means clustering for exploratory employee segmentation
- Logistic Regression, Random Forest, and Gradient Boosting classification
- Hyperparameter tuning with cross-validation
- Model evaluation using precision, recall, F1-score, and ROC-AUC
- Feature-importance analysis and illustrative risk stratification

## Results

The selected **Gradient Boosting Classifier** achieved the following performance on the held-out test set:

| Metric | Score |
|---|---|
| Precision | 0.910 |
| Recall | 0.920 |
| F1-score | 0.915 |
| ROC-AUC | 0.980 |

Gradient Boosting was selected using a recall-focused criterion, prioritizing the identification of employees at risk of leaving.

The analysis identified satisfaction level and time spent with the company as the strongest predictive features. These associations should not be interpreted as causal relationships.

## Repository Structure

```text
employee-turnover-analytics/
├── employee-turnover-analytics.ipynb
├── data/
│   └── P1Dataset_HR_comma_sep.csv
├── outputs/
│   └── feature_importance_gradient_boosting.csv
└── artifacts/
    ├── final_gradient_boosting_model.joblib
    └── model_feature_columns.joblib
```

## Intended Use and Limitations

This project demonstrates a potential application of predictive analytics to employee-retention analysis. Its risk categories are illustrative and have not been validated for operational deployment.

Predictions should support human review rather than automated employment decisions. Real-world implementation would require further validation, fairness assessment, appropriate data governance, and organizational oversight.

## Project Context

Developed as a Machine Learning final project for the Purdue University / IBM AI and Machine Learning Certificate program, delivered through Simplilearn. Refined for professional portfolio presentation.