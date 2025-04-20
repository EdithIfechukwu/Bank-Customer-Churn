# Predicting Bank Customer Churn with Machine Learning

This project applies machine learning techniques to predict customer churn for a retail bank. The model helps identify high-risk customers who are likely to leave, enabling proactive retention strategies.

## Overview

- **Model Used:** Random Forest
- **Tech Stack:** Python, Pandas, scikit-learn, XGBoost, SHAP, Streamlit (optional)  
- **Dataset:** Public synthetic dataset simulating European bank customer profiles  
- **Problem Type:** Binary Classification  

## Business Context

Customer churn is a major challenge in the banking sector, costing institutions billions annually. This project was built to empower retention teams with predictive tools to prioritize customer outreach and reduce churn rates.

## Features Used

- Credit Score  
- Age  
- Balance  
- Tenure  
- Number of Products  
- Has Credit Card  
- Is Active Member  
- Estimated Salary  
- Geography & Gender

## Methodology

1. **Exploratory Data Analysis (EDA):**  
   Uncovered trends like older customers and high balance accounts churning more.

2. **Feature Engineering:**  
   One-hot encoding of categorical variables (e.g., Geography), standardization of numeric features.

3. **Modeling:**  
   - Trained Random classifier  
   - Used GridSearchCV for hyperparameter tuning  
   - Evaluated with AUC-ROC, precision, and recall

4. **Interpretability:**  
   Used SHAP to understand feature impact and individual prediction explanations.

## Model Performance

- **Accuracy:** 86%  
- **Precision:** 82%  
- **Recall:** 78%  
- **AUC-ROC:** 0.90

## SHAP Explanation

![SHAP summary plot]

The SHAP plot revealed:
- Age and account activity were top indicators
- Inactive users with low tenure were highly likely to churn

## Impact

- Created a web-based dashboard prototype for customer retention teams  
- Helped simulate scenarios for proactive retention campaigns  
- Encouraged more data-driven customer loyalty initiatives

## Next Steps

- Integrate model into CRM systems  
- Automate real-time churn scoring via API  
- Apply clustering for customer segmentation

## Repository Structure

- `notebooks/`: EDA and model training notebooks  
- `models/`: Trained model pickle files  
- `src/`: Scripts for preprocessing and model evaluation  
- `streamlit_app/`: Simple UI for model interaction (optional)  
- `reports/`: Visuals and SHAP plots  

## Author
Ifechukwu Ukatu
