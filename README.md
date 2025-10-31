# Predictive Analyticsin the UPI Ecosystem : Demand Forecasting and Fraud Detection

## Introduction :
This project applies predictive analytics to the Indian UPI (Unified Payments Interface) ecosystem to forecast transaction demand and detect potential fraud. It combines **Simple Linear Regression** for demand forecasting and **Logistic Regression** for fraud classification, providing a dual perspective on digital payment trends and risks.

## Objectives
- Forecast UPI transaction demand using **Simple Linear Regression (SLR)**.
- Detect potential fraudulent transactions using **Logistic Regression**.
- Evaluate model performance using R², RMSE (for regression) and accuracy, precision, recall, F1-score (for classification).
- Generate actionable insights for fintech and policymakers.


## Datasets 
### UPI Demand Forecasting Dataset
- 84 monthly observations (2018–2024) with 11 features.
- Features: GDP growth, smartphone penetration, internet users, POS terminals, PMJDY accounts, repo rate, etc.
- Source: RBI, NPCI, MoSPI, and public records.

### UPI Fraud Detection Dataset
- 10,000 transaction records across 19 attributes.
- Features: transaction amount, frequency, device ID, location, failed attempts, etc.
- Source: Kaggle & Simulated dataset (for testing the model).
