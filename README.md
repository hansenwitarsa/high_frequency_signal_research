# Predictive Signal Analysis for Short-Horizon Market Returns

## Overview
This project investigates predictive signals for short-horizon asset returns using high-frequency market data. The objective is to identify features with predictive power, construct a composite trading signal, and evaluate its robustness across different market conditions.

The workflow follows a typical quantitative research pipeline used in systematic trading and financial modeling.

---

## Methodology

### 1. Feature Predictiveness Analysis
Initial feature screening is performed using the **Information Coefficient (IC)** to measure the correlation between each feature and future returns. This step identifies candidate predictors with potential forecasting power.

### 2. Prediction Horizon Analysis
Signal performance is evaluated across multiple time horizons to study **signal decay** and determine the most effective prediction horizon for short-term forecasting.

### 3. Composite Signal Construction
Selected features are combined using **linear regression** to build a composite signal. Feature selection and coefficient analysis are used to identify the most informative predictors.

### 4. Signal Evaluation
The composite signal is evaluated using several quantitative metrics:

- **Information Coefficient (IC)**
- **R² (coefficient of determination)**
- **Daily IC distribution**
- **Quantile return analysis**

### 5. Robustness and Stability Analysis
To assess signal reliability, the following diagnostics are performed:

- **Rolling IC analysis** to examine time-varying predictive performance  
- **Quantile portfolio returns** to evaluate economic significance  
- **Regime analysis** to study performance under different market conditions  

---

## Results
The final composite signal demonstrates consistent predictive power across the selected horizon and maintains stable performance across different market regimes. Quantile return analysis shows clear separation between high- and low-signal portfolios, indicating meaningful predictive structure in the selected features.

---

## Tools and Technologies

- Python  
- pandas  
- numpy  
- scikit-learn  
- matplotlib  

---

## Repository Structure
