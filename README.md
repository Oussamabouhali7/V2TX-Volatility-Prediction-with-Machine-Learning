# 📈 V2TX Volatility Prediction — Machine Learning

## 📌 Overview

This project focuses on predicting the **V2TX (VSTOXX)** volatility index using Machine Learning and time-series analysis.

V2TX represents the implied volatility of the **EURO STOXX 50**. The project analyzes historical volatility data and develops predictive models to forecast future V2TX levels.

The dataset contains **6,926 daily observations** covering the period from **January 1999 to March 2026**.

## 🎯 Objectives

- Analyze the historical behavior of V2TX
- Engineer predictive time-series features
- Compare different Machine Learning models
- Identify volatility regimes
- Evaluate model forecasting performance
- Generate short-term and 30-day volatility forecasts

## 📊 Dataset

| Property | Value |
|---|---|
| Index | V2TX (VSTOXX) |
| Underlying | EURO STOXX 50 |
| Period | 1999-01-04 → 2026-03-18 |
| Observations | 6,926 daily observations |
| Prediction Horizon | J+1 |
| Engineered Features | 39 |

## 🔧 Feature Engineering

The project uses **39 engineered variables**, including:

- Temporal lags: 1, 2, 3, 5, 10, 21 and 63 days
- Moving averages: 5, 10, 21, 63 and 126 days
- Rolling realized volatility
- RSI
- Bollinger Bands
- Z-score
- Momentum
- Log-returns
- Volatility regimes
- Calendar variables

### Volatility Regimes

The analysis considers four volatility regimes:

- Low
- Normal
- Stress
- Crisis

## 🤖 Machine Learning Models

The project compares several regression approaches:

1. Naive Baseline
2. Ridge Regression
3. Lasso Regression
4. Random Forest
5. Gradient Boosting Machine (GBM)
6. Other Machine Learning models

Models are trained and evaluated using a time-series approach while preserving the chronological order of observations.

## 📈 Forecasting

The project generates V2TX forecasts by comparing predictions from different Machine Learning models.

The final visualization includes:

- Historical V2TX values
- Random Forest predictions
- GBM predictions
- Model consensus
- Prediction confidence interval
- Volatility thresholds
- 30-day forward forecast

The final forecast visualization uses the latest known V2TX value and projects the expected volatility over the following 30 days.

## 📊 Visualizations

The project includes visualizations for:

- Historical V2TX evolution
- Machine Learning predictions
- 30-day forecast
- Model consensus
- Prediction intervals
- Residual analysis
- Volatility regimes

## 🛠️ Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Jupyter Notebook
- Machine Learning
- Time-Series Analysis
