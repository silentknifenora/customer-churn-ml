# Telco Customer Churn Prediction & Risk Segmentation
- Project Overview

Customer churn directly impacts recurring revenue in subscription-based businesses.

This project builds machine learning classification models to predict high-risk telecom customers and translate model outputs into actionable retention strategies.

Two models were developed and compared:

Logistic Regression – interpretable baseline model

Random Forest – non-linear ensemble model

The objective was not only to maximize overall accuracy, but to improve churn recall, ensuring high-risk customers are correctly identified for proactive intervention.

# Business Objectives

Identify customers at high risk of churn

Improve recall for the churn (minority) class

Understand key drivers influencing churn behavior

Enable data-driven customer retention strategies

# Tech Stack

Python
Pandas & NumPy
Scikit-learn
Matplotlib & Seaborn

# Dataset

Telco Customer Churn Dataset
7,032 customer records

Key Features:

Demographics: Gender, SeniorCitizen, Partner, Dependents

Account Information: Tenure, Contract Type, Payment Method

Financial Metrics: MonthlyCharges, TotalCharges

Service Usage: InternetService

Target Variable: Churn (Yes = 1, No = 0)

# Methodology
1. Data Preprocessing

Removed non-informative identifiers (customerID)

Converted churn to binary format (1 = Yes, 0 = No)

Applied One-Hot Encoding to categorical variables

Standardized numeric features using StandardScaler

2. Train-Test Split

80/20 split to evaluate generalization performance

3. Model Development
Model 1: Logistic Regression

Interpretable linear classifier

Baseline performance benchmark

Accuracy ≈ 78.7%

Model 2: Random Forest

Captures non-linear feature interactions

Reduced bias compared to baseline

Accuracy ≈ 84–86%

4. Model Evaluation

Confusion Matrix

Precision, Recall, F1-score

Emphasis on Churn Recall (minority class performance)

5. Feature Importance Analysis

Extracted top churn drivers using Random Forest

Identified variables contributing most to churn probability

# Key Results
Model	Accuracy	Churn Recall	Churn Precision
Logistic Regression	78.7%	52%	62%
Random Forest	~84%	65–70%	68%
# Top Churn Drivers Identified:

Contract Type

Monthly Charges

Tenure

Total Charges

Internet Service

Short-tenure customers with higher monthly charges and month-to-month contracts exhibited the highest churn probability.

# Business Impact

This model enables:

Proactive retention targeting

Risk-based customer segmentation

Prioritized outreach to high-risk accounts

Data-backed churn mitigation strategies

Revenue protection through early intervention

# Model Performance Visuals

![Confusion Matrix](images/confusion_matrix.png)

Confusion Matrix

![Feature Importance](images/feature_importance.png)

Feature Importance

# Skills Demonstrated

End-to-End Machine Learning Workflow

Data Cleaning & Feature Engineering

Classification Modeling

Model Evaluation & Trade-off Analysis

Translating ML Outputs into Business Insights

# Author

Neha Raut


