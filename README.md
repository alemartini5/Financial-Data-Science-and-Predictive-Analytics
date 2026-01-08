# Quantitative Analysis and Stochastic Modeling: A Financial Engineering Approach


This repository contains an end-to-end framework for financial data science, developed as a final project for the **Business Intelligence for Financial Services** course. The project integrates traditional econometric models, machine learning, and mathematical optimization to analyze and forecast financial markets.

## Project Overview

The core objective of this study is to bridge the gap between raw financial data and actionable insights. The pipeline covers the entire workflow of a Data Scientist/Quantitative Analyst:
1. **Data Engineering**: Automated ingestion and cleaning of multi-asset datasets using `yfinance` and `pandas`.
2. **Statistical Analysis**: Deep dive into returns distributions, stationarity tests (ADF), and normality tests (Jarque-Bera).
3. **Forecasting**: Comparative analysis between stochastic models (ARIMA/Auto-ARIMA) and non-linear models.
4. **Strategy Backtesting**: Quantitative evaluation of trading rules (SMA, Mean Reversion, Random Forest) with a focus on risk-adjusted returns and Walk-Forward robustness.
5. **Modern Portfolio Theory**: Numerical optimization for risk-adjusted asset allocation (Markowitz).

---

##  Repository Structure

- report/ -> RelazioneBISF_AlessioMartini.pdf (Detailed 24-page technical report; **Note: Currently in Italian**)
- notebooks/ -> BISF_Project_AlessioMartini.ipynb (Full Python implementation)
- README.md -> Project documentation
- requirements.txt -> Dependencies list

---

##  Key Technical Features

### 1. Time-Series Forecasting (ARIMA & Auto-ARIMA)
Implementation of ARIMA models for signal extraction. The study includes a rigorous analysis of residuals and error metrics (RMSE, MAE). Analysis of the "low predictability" nature of financial returns compared to price trends, emphasizing the limits of linear stochastic modeling.

### 2. Machine Learning for Trading (Random Forest)
Development of a Random Forest Classifier to identify market regimes and generate signals based on technical indicators like lagged returns, moving averages, and volatility proxies. Evaluation via robust comparison against a Buy & Hold benchmark.

### 3. Factor Models (CAPM & Fama-French)
Quantifying asset risk and exposure through CAPM (Single-factor Beta estimation) and Fama-French 3-Factors (evaluating Market, Size/SMB, and Value/HML premiums using multivariate OLS regressions).

### 4. Portfolio Optimization & Efficient Frontier
Numerical resolution of asset allocation problems. Comparison between Historical Expectations and CAPM-derived expectations to assess model sensitivity and out-of-sample stability.

---

##  Technical Report
A comprehensive 24-page technical report is available in the /report folder. It provides a scientific discussion of:
- Data stationarity and statistical properties of financial time series.
- Methodology for Out-of-sample (OOS) validation and backtesting.
- Critical assessment of model limitations (e.g., ARIMA's performance during market shocks).

---

##  Author
- Alessio Martini
- University Project: Business Intelligence for Financial Services
