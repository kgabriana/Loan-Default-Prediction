Overview

Loan defaults cause significant financial losses for lenders. Traditional credit scoring methods lack nuance in borrower behavior, leading to suboptimal risk assessments. This project implements a machine learning-driven approach to predict loan default risk and improve lending decisions.

Project Goals
- Develop a predictive model to identify high-risk loan applicants.
- Determine borrower features that strongly indicate default risk.
- Optimize recall for defaulters to reduce financial loss.

Dataset & Preprocessing
- Exploratory Data Analysis (EDA):- Addressed missing values, skewness, and scaling issues.
- Boxplots and correlation matrices analyzed key features influencing defaults.

Feature Engineering:
- Property Feature: Combines loan, value, and mortgage due effects.
- Financial Stability Score: Measures borrower stability via credit age and number of lines.

Model Selection & Training
- Evaluated Decision Trees, Random Forest, and XGBoost.
- XGBoost chosen for best recall (89.2%) in predicting defaulters.
- Hyperparameter tuning using RandomizedSearchCV with recall scoring.
- SMOTE applied to handle class imbalance before model training.

Decision Threshold Adjustment
- Adjusted classification threshold from 0.50 to 0.49 to boost recall.
- Precision-Recall tradeoff monitored for optimal risk management.


SHAP Explainability: 
- Debt-to-Income Ratio (DEBTINC) strongly correlates with default risk.
- Delinquency History (DELINQ) indicates likelihood of future defaults.
- Financial Stability Score impacts default probability.

Business Impact
- Loan default detection enabled cost savings of $8.98M.
- SHAP dashboard supports transparent credit decisions.
- Model seamlessly integrates into loan origination systems.






