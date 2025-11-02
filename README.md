Loan Credit Risk Analysis Identifying Patterns Behind High-risk Loan Applications

I. Project Overview
This project aims to build a machine learning model to classify credit applicants into risk categories using structured financial data. The CatBoost algorithm was selected for its ability to handle categorical features, class imbalance, and non-linear relationships.

II. Key Objectives
Perform exploratory data analysis (EDA) to uncover patterns in high-risk applicants.
Engineer meaningful features such as ratio-based indicators.
Tune hyperparameters to improve minority class detection.
Evaluate model performance across multiple thresholds.
Generate actionable insights for business deployment.

III. Data Preprocessing
Feature engineering:
CREDIT_INCOME_RATIO
ANNUITY_INCOME_RATIO
CREDIT_GOODS_RATIO
Class imbalance handled via dynamic class weights.
Threshold optimization performed using F1, Precision, Recall curves.

IV. Model Performance
Algorithm: CatBoostClassifier
Threshold: 0.7 (optimized via metric trade-off)
Accuracy: 73%
Precision (class 1): 0.15
Recall (class 1): 0.49
AUC: 0.67

V. Visualizations
Confusion Matrix with annotated TP, FP, TN, FN
ROC Curve with AUC
Threshold vs Metric trade-off chart

VI. Insights
Working class applicants show strong correlation with high-risk profiles due to annuity and income ratios.
Loan type (cash vs revolving) has minimal impact on risk classification.
Numerical features are more informative than encoded Boolean flags.
CatBoost handles minority class better than logistic regression, despite lower precision.

VII. Actionable Business Plans
Use model for pre-screening and credit simulation.
Prioritize risk management on cash loans due to applicant volume.
Monitor model drift and retrain periodically.
Consider synthetic oversampling for minority class enhancement.

🚀 Deployment Potential
This model is suitable for integration into credit scoring pipelines, risk dashboards, or business decision support systems.
