# Predictive Analyticsin the UPI Ecosystem : Demand Forecasting and Fraud Detection  (On-going)

## 🧾 Introduction :
This project applies predictive analytics to the Indian UPI (Unified Payments Interface) ecosystem to forecast transaction demand and detect potential fraud. It combines **Simple Linear Regression** for demand forecasting and **Logistic Regression** for fraud classification, providing a dual perspective on digital payment trends and risks.



## 📂 Repository Structure
```
├── data/
│   ├── UPI Demand Prediction data.xlsx
│   ├── UPI Fraud Prediction data.csv
│   ├── UPI Fraud Prediction data.csv
├── notebooks/
│   ├── demand_forecasting.ipynb
│   ├── fraud_detection.ipynb
├── visuals/
│   ├── correlation_heatmap.png
│   ├── roc_curve.png
├── Report_Writing_trial.pdf
└── README.md
```

## 🎯 Objectives
- Forecast UPI transaction demand using **Simple Linear Regression (SLR)**.
- Detect potential fraudulent transactions using **Logistic Regression**.
- Evaluate model performance using R², RMSE (for regression) and accuracy, precision, recall, F1-score (for classification).
- Generate actionable insights for fintech and policymakers.


## 📊 Datasets 
#### UPI Demand Forecasting Dataset
- 84 monthly observations (2018–2024) with 11 features.
- Features: GDP growth, smartphone penetration, internet users, POS terminals, PMJDY accounts, repo rate, etc.
- Source: RBI, NPCI, MoSPI, and public records.

#### UPI Fraud Detection Dataset
- 10,000 transaction records across 19 attributes.
- Features: transaction amount, frequency, device ID, location, failed attempts, etc.
- Source: Kaggle & Simulated dataset (for testing the model).

## ⚙️ Methodology
1. **Data Collection & Preprocessing**
   - Handled missing values, encoded categorical data, scaled features.
2. **Exploratory Data Analysis**
   - Detected outliers, correlations, and feature relationships.
3. **Model Building**
   - Simple Linear Regression for demand forecasting.
   - Logistic Regression for fraud detection.
4. **Model Evaluation**
   - SLR: R², RMSE.
   - Logistic Regression: Accuracy, Precision, Recall, F1-score, ROC-AUC.


## 📈 Exploratory Data Analysis
- No missing values in either dataset.
- Detected outliers using boxplots and Z-scores.
- High correlation between internet usage, smartphone penetration, and UPI demand.
- Visualizations: heatmaps, scatterplots, boxplots.


## 🤖 Modeling & Results
#### UPI Demand Forecasting (Simple Linear Regression)
- **Significant Predictors:** Smartphone Penetration (p<0.001), Internet Users (p=0.005), PMJDY Accounts (p=0.017)
- **Model Performance:** R² = 0.998, Adj R² = 0.997
- **Predicted UPI Demand (2025):** ≈ 272.25 million transactions

#### UPI Fraud Detection (Logistic Regression)
- **Significant Predictors:** FailedAttempts, LocationRiskScore, Amount
- **Model Accuracy:** 83%
- **Precision (Fraud):** 0.78 | **Recall (Fraud):** 0.80 | **F1-score:** 0.79
- Detected 84 users with >70% fraud probability.

## 🔍 Key Insights 
- Smartphone and internet penetration are the strongest drivers of UPI growth.
- Seasonal spikes correspond with festivals and e-commerce events.
- Failed login attempts and high-risk geolocations are major fraud predictors.
- Predictive analytics can significantly improve proactive fraud monitoring.


## 💡 Conclusions 
**Conclusions:**
- Predictive analytics provides actionable insights for both demand and fraud patterns.
- Regularized regression models improve stability and interpretability.

**Recommendations:**
- Enhance digital literacy and smartphone access.
- Implement geolocation-based fraud scoring.
- Flag high-value transactions for verification.
- Continuously retrain models with new data.


## ⚠️ Limitations & Future Work
- Linear assumptions may not capture all relationships.
- Some behavioral and contextual data were unavailable.
- Future models can use non-linear techniques (Random Forest, XGBoost) and real-time streaming data.
