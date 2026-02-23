\# Telco Customer Churn Prediction \& Risk Segmentation

\- Project Overview



Customer churn directly impacts recurring revenue in subscription-based businesses.

This project builds predictive models to identify telecom customers at high risk of churn and translates model outputs into actionable retention strategies.



Two classification models were developed:



Logistic Regression – baseline linear model



Random Forest – non-linear ensemble model



The goal was not only to maximize accuracy, but to improve churn recall, ensuring high-risk customers are correctly identified.



\# Tech Stack



Python | Pandas | NumPy | Scikit-learn | Matplotlib | Seaborn



\# Key ML Concepts



Feature Engineering



One-Hot Encoding



Feature Scaling



Model Evaluation (Precision, Recall, F1)



Feature Importance Analysis



\# Dataset



Telco Customer Churn dataset – 7,032 customers



Key variables include:



Demographics: Gender, SeniorCitizen, Partner, Dependents



Account Info: Tenure, Contract type, Payment method



Financial Metrics: MonthlyCharges, TotalCharges



Service Usage: InternetService



Target Variable: Churn (Yes=1, No=0)



\# Methodology

1\. Data Preprocessing



Removed non-informative identifiers (customerID)



Converted Churn into binary format (Yes=1, No=0)



Applied One-Hot Encoding to categorical variables



Standardized numeric features using StandardScaler



2\. Train-Test Split



80/20 split to evaluate model generalization



3\. Model Development



Model 1: Logistic Regression



Baseline linear classifier



Interpretable coefficients



Accuracy ≈ 78.7%



Model 2: Random Forest



Captures non-linear feature interactions



Reduced bias compared to baseline



Accuracy ≈ 83–86%



4\. Model Evaluation



Confusion Matrix



Precision, Recall, F1-score



Focus on churn recall (minority class performance)



5\. Feature Importance Analysis



Extracted top churn drivers using Random Forest



Helps understand which variables contribute most to churn



\# Key Results

Model	Accuracy	Churn Recall	Churn Precision

Logistic Regression	78.7%	52%	62%

Random Forest	~84%	65–70%	68%



Top Churn Drivers Identified:



Contract Type



Monthly Charges



Tenure



Total Charges



Internet Service



Short-tenure customers with higher monthly charges and month-to-month contracts had the highest churn probability.



\# Business Impact



Enables proactive retention targeting



Supports risk-based customer segmentation



Helps prioritize outreach to high-risk accounts



Provides interpretable drivers for churn mitigation strategies



Allows businesses to intervene before revenue loss



\# Model Performance Visuals

Confusion Matrix



Feature Importance



\# Skills Demonstrated



End-to-End ML Workflow



Data Cleaning \& Feature Engineering



Classification Modeling



Model Evaluation \& Performance Tradeoffs



Translating ML Output into Business Strategy



\# Author



Neha Raut

