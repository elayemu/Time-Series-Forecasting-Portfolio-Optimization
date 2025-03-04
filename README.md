# Time Series Forecasting for Portfolio Optimization

## Overview
This project applies time series forecasting techniques to historical financial data to optimize portfolio management for GMF Investments. The goal is to predict market trends, optimize asset allocation, and enhance portfolio performance by minimizing risks and capitalizing on market opportunities.

## Business Context
GMF Investments provides personalized portfolio management using data-driven insights. By forecasting stock prices and market trends, we enable clients to make informed investment decisions.

## Data Sources
- **Tesla (TSLA)**: High-growth, high-risk stock.
- **Vanguard Total Bond Market ETF (BND)**: Stable bond ETF.
- **S&P 500 ETF (SPY)**: Diversified, moderate-risk market exposure.

Data is fetched from **Yahoo Finance** using the `yfinance` Python library and covers the period **January 1, 2015 – January 31, 2025**.

## Project Tasks
### 1. Data Preprocessing & Exploration
- Extract historical stock data using `yfinance`.
- Clean and preprocess data: handle missing values, normalize features.
- Conduct **Exploratory Data Analysis (EDA)**:
  - Plot closing prices and daily returns.
  - Analyze volatility, rolling statistics, and seasonality.
  - Perform outlier detection.

### 2. Time Series Forecasting Models
- Develop forecasting models for Tesla stock prices:
  - **ARIMA** – Statistical approach for univariate time series.
  - **SARIMA** – Seasonal variation of ARIMA.
  - **LSTM** – Deep learning model capturing long-term dependencies.
- Train and evaluate models using:
  - Mean Absolute Error (MAE)
  - Root Mean Squared Error (RMSE)
  - Mean Absolute Percentage Error (MAPE)

### 3. Forecasting Market Trends
- Generate **6-12 month stock price forecasts**.
- Compare actual vs. predicted prices.
- Analyze trends, volatility, and risks.
- Include **confidence intervals** for predictions.

### 4. Portfolio Optimization
- Build a **portfolio of three assets (TSLA, BND, SPY)**.
- Compute **annual return, risk, and Sharpe Ratio**.
- Use a **covariance matrix** to assess asset correlations.
- Optimize portfolio weights for **maximum returns with minimal risk**.
- Analyze **risk-adjusted returns, expected volatility, and VaR**.

## Installation & Usage
### Prerequisites
Ensure you have Python installed (compatible with Windows Command Prompt).

Install dependencies:
```sh
pip install yfinance numpy pandas matplotlib seaborn scikit-learn statsmodels pmdarima tensorflow
