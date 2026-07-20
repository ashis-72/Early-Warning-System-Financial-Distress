# 📊 Early Warning System for Financial Distress Prediction

An interpretable machine learning framework for predicting the future financial distress of Indian publicly listed companies using accounting-based financial indicators.

---

## 📌 Project Overview

Financial distress can significantly impact investors, lenders, regulators, and corporate stakeholders. Identifying financially vulnerable firms before distress occurs enables proactive decision-making and risk mitigation.

This project develops an **Early Warning System (EWS)** that predicts future financial distress using financial statement data from Indian publicly listed companies. The framework combines statistical feature selection, machine learning, explainable AI, and probability-based risk assessment to produce accurate and interpretable predictions.

---

## 🎯 Objectives

- Predict future financial distress of publicly listed Indian companies.
- Construct an interpretable machine learning model using accounting-based financial indicators.
- Compare multiple classification algorithms.
- Address class imbalance using SMOTENC.
- Explain model predictions using SHAP.
- Develop an Early Warning Dashboard for practical decision support.

---

## 📂 Dataset

The dataset was constructed using financial statement information collected from **Screener.in** for companies listed in the **Nifty 500 Index** using Web Scraping.

**Data Sources**

- National Stock Exchange (NSE)
- Screener.in

The dataset contains company-level financial variables including:

- Sales
- Net Profit
- Cash Flow from Operations
- Total Assets
- Total Liabilities
- Borrowings
- Equity Capital
- Reserves
- Interest Expense
- Operating Profit
- Investments
- Fixed Assets
- and other financial indicators.

The target variable was created using accounting-based financial distress criteria.

---

## 🛠 Methodology

The project follows the following workflow:

```
Data Collection
        │
        ▼
Data Cleaning & Preprocessing
        │
        ▼
EDA
        │
        ▼
Feature Engineering
        │
        ▼
Feature Selection
(Mann–Whitney U Test → Correlation → VIF → LASSO Validation)
        │
        ▼
SMOTENC
        │
        ▼
Machine Learning Models
(Logistic Regression, Decision Tree, Random Forest,
XGBoost, LightGBM, CatBoost)
        │
        ▼
Hyperparameter Optimization (Optuna)
        │
        ▼
Threshold Optimization
        │
        ▼
SHAP Explainability
        │
        ▼
Early Warning Dashboard
```

---

## 🤖 Machine Learning Models

The following classification models were evaluated:

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost
- LightGBM
- CatBoost

Model performance was evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Precision–Recall AUC (Primary Metric)

---

## 🏆 Final Model

**Optimized Random Forest**

Evaluation Metrics:

| Metric | Value |
|---------|------:|
| PR-AUC | **0.752** |
| ROC-AUC | **0.988** |
| F1-score | **0.729** |

Random Forest was selected due to its superior performance under class imbalance and strong predictive capability.

---

## 🔍 Model Interpretability

Model predictions were interpreted using **SHAP (SHapley Additive Explanations)**.

Key predictors of financial distress include:

- Interest Coverage
- Return on Assets (ROA)
- Net Profit
- Operating Profit
- Equity Ratio
- CFO to Assets

This improves transparency and provides financial insights into the model's decision-making process.

---

## 📈 Key Features

- Financial statement-based prediction framework
- Statistical feature selection
- SMOTENC for class imbalance
- Hyperparameter optimization using Optuna
- SHAP explainability
- Threshold optimization
- Early Warning Dashboard
- Forward-looking financial distress prediction

---



---

## 💻 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- LightGBM
- CatBoost
- SHAP
- Optuna
- Matplotlib
- SciPy
- Statsmodels

---

## 🚀 Future Improvements

- Incorporate market-based indicators
- Include macroeconomic variables
- Explore deep learning models
- Develop a real-time web dashboard
- Extend the framework to international markets

---

## 📚 References

- Altman (1968)
- Beaver (1966)
- Ohlson (1980)
- Lundberg & Lee (2017)
- Pedregosa et al. (2011)

---

## 👤 Author

**Ashis Pal**

Master's in Applied Quantitative Finance  
Madras School of Economics

---
