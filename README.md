# Customer Churn Prediction in Telecommunications

## Overview

This project focuses on predicting customer churn in the telecommunications industry using machine learning techniques. The objective is to identify customers who are likely to leave (churn) and support proactive retention strategies based on data-driven insights.

## Objectives

* Analyze customer behavior and churn patterns
* Build predictive models to estimate churn probability
* Identify key factors influencing customer churn
* Support business decision-making through customer segmentation

## Dataset

The dataset contains customer-level information including:

* Demographics (e.g., gender, senior citizen status)
* Account details (contract type, tenure, payment method)
* Service usage (internet services, streaming, support, etc.)
* Financial variables (Monthly Charges, Total Charges)

## Data Preparation

Key preprocessing steps included:

* Converting `TotalCharges` to numeric and handling missing values
* Encoding categorical variables using One-Hot Encoding
* Feature engineering:

  * **ServicesCount** (number of subscribed services)
  * **CLV (Customer Lifetime Value)**
  * **CLV Segmentation**
* Splitting data into training and testing sets using stratification

## Models Used

Two classification models were implemented:

### Logistic Regression

* Interpretable model to understand feature impact
* Threshold optimization to improve recall of churners
* ROC AUC ≈ 0.84

### Random Forest

* Ensemble model capturing non-linear relationships
* Handles feature interactions effectively
* Provides feature importance ranking

## Evaluation Metrics

* Accuracy
* Precision & Recall
* F1-score
* ROC AUC
* Confusion Matrix

Threshold tuning was applied to balance precision and recall and align with business objectives.

## Key Insights

* Customers with **month-to-month contracts** show the highest churn rate
* **Electronic check payment method** is strongly associated with churn
* Longer tenure significantly reduces churn probability
* High-value customers (based on CLV) require targeted retention strategies

## Business Impact

The model enables:

* Identification of **high-risk, high-value customers**
* Optimization of retention campaigns
* Reduction of revenue loss due to churn

## Tools & Technologies

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn

## Project Structure

* `predicting_customer_churn.ipynb` – full analysis and modeling
* Data preprocessing, EDA, modeling, and evaluation included in notebook

## Conclusion

This project demonstrates how machine learning can be applied to predict customer churn and generate actionable insights. By combining predictive modeling with business-oriented metrics such as CLV, the solution provides practical value for customer retention strategies.
