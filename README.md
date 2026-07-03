![Python](https://img.shields.io/badge/Python-3.11-blue)
![XGBoost](https://img.shields.io/badge/XGBoost-ML-success)
![PyPortfolioOpt](https://img.shields.io/badge/PyPortfolioOpt-Optimization-orange)
![License](https://img.shields.io/badge/License-MIT-green)
# FinOptix: Machine Learning Stock Selection & Portfolio Optimization

An end-to-end quantitative investment framework that integrates **Machine Learning**, **Fundamental Analysis**, **Factor Investing**, and **Modern Portfolio Theory** to automate stock selection and construct risk-optimized portfolios.

The framework predicts stock returns using **XGBoost**, ranks stocks using a hybrid scoring mechanism, optimizes allocations with the **Black-Litterman** and **Markowitz Mean-Variance Optimization** models, and evaluates performance through historical backtesting.

---

## Overview

The project follows the complete quantitative investment workflow:

```
Historical Market Data
        │
        ▼
 Feature Engineering
        │
        ▼
 XGBoost Return Prediction
        │
        ▼
 Fundamental Stock Scoring
        │
        ▼
 Top Stock Selection
        │
        ▼
 Black-Litterman Portfolio
        │
        ▼
 Mean-Variance Optimization
        │
        ▼
 Historical Backtesting
        │
        ▼
 Performance Evaluation
```

---

# Features

## Machine Learning Stock Selection

- XGBoost regression model for stock return prediction
- Individual models trained for each NIFTY 50 stock
- Out-of-sample prediction on unseen market data
- Correlation and RMSE based evaluation

---

## Feature Engineering

Generated multiple technical indicators including

- Daily Returns
- Rolling Volatility
- Moving Averages (10-Day & 50-Day)
- Momentum Indicators
- Bollinger Bands
- Lagged Returns
- Volume Correlation

---

## Fundamental Analysis

Stocks are ranked using a weighted combination of

- Expected Return (Predicted by XGBoost)
- Price-to-Earnings Ratio
- Debt-to-Equity Ratio
- Market Capitalization

The framework selects the **Top 20 stocks** with the highest composite scores.

---

## Portfolio Optimization

Implemented multiple quantitative portfolio construction techniques

- Markowitz Mean-Variance Optimization
- Black-Litterman Bayesian Portfolio Model
- Fama-French Three-Factor Model
- Efficient Frontier Analysis
- Maximum Sharpe Ratio Optimization

---

## Risk Management

The project incorporates practical trading constraints including

- Long & Short Positions
- Dynamic Portfolio Allocation
- Risk-adjusted Optimization
- Historical Portfolio Simulation

---

# Data

**Universe**

- NIFTY 50 Constituents

**Historical Data Source**

- Yahoo Finance (yFinance API)

**Training Period**

- March 2022 – May 2024

**Prediction Period**

- June 2024 – July 2025

---

# Technologies Used

- Python
- Pandas
- NumPy
- XGBoost
- Scikit-Learn
- PyPortfolioOpt
- Matplotlib
- Yahoo Finance API

---

# Workflow

### 1. Data Collection

- Download historical prices
- Retrieve company fundamentals
- Clean missing observations

### 2. Feature Engineering

Generate predictive technical indicators and market statistics.

### 3. Machine Learning

Train XGBoost regression models independently for every stock.

### 4. Stock Ranking

Combine

- ML predicted returns
- P/E score
- Debt-to-Equity score
- Market Capitalization score

into a weighted ranking model.

### 5. Portfolio Construction

Generate optimal portfolio weights using

- Black-Litterman Model
- Mean-Variance Optimization

### 6. Evaluation

Compare optimized portfolio against an equal-weight benchmark using historical simulations.

---

# Results

## Stock Selection

- Successfully developed a hybrid stock ranking framework combining **machine learning predictions** with **fundamental financial metrics**.
- Generated expected returns using **XGBoost regression** trained on engineered technical indicators.
- Ranked and selected the **Top 20 NIFTY 50 stocks** through a weighted multi-factor scoring model.

---

## Portfolio Optimization

The selected stocks were optimized using the **Black-Litterman Bayesian framework**, followed by **Markowitz Mean-Variance Optimization** to generate a risk-adjusted portfolio with maximum Sharpe Ratio.

The optimized portfolio was benchmarked against an equal-weight portfolio using historical simulations.

---

## Visualizations

The project includes

- Actual vs Predicted Returns
- Top Stock Rankings
- Fundamental Metric Comparisons
- Portfolio Allocation Comparison
- Portfolio Performance Curves
- Correlation & RMSE Analysis
- Efficient Frontier

---

# Future Improvements

- Transaction Cost Modeling
- Dynamic Portfolio Rebalancing
- Macroeconomic Indicators
- Sentiment Analysis
- Sector Rotation Models
- Reinforcement Learning based Portfolio Allocation
- Live Paper Trading Support

---

# Repository Structure

```
├── data/
├── notebooks/
├── models/
├── reports/
├── plots/
├── utils/
├── README.md
└── requirements.txt
```

---

# Key Concepts

- Machine Learning for Financial Forecasting
- Quantitative Stock Selection
- Feature Engineering
- Factor Investing
- Black-Litterman Portfolio Optimization
- Markowitz Mean-Variance Optimization
- Fama-French Three-Factor Model
- Efficient Frontier
- Risk-Adjusted Portfolio Construction
- Historical Backtesting

---

## Acknowledgements

This project was developed as part of the **Finance and Data Analytics Club (FinOptix), IIT Kanpur**, combining quantitative finance, machine learning, and portfolio optimization techniques for systematic investment analysis.
