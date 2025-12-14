# Stock Price Prediction Using Machine Learning and Deep Learning

## Overview
This project implements a stock price prediction system using historical market data and technical indicators. It combines traditional machine learning and deep learning approaches to compare performance and behavior on time-series financial data. Stock data is fetched dynamically using Yahoo Finance and processed to extract meaningful indicators before training the models.

## Models Used
- **Random Forest Regressor**
  - Ensemble-based machine learning model
  - Captures non-linear relationships between technical indicators and stock prices

- **LSTM (Long Short-Term Memory) Network**
  - Deep learning model designed for sequential data
  - Learns temporal dependencies in financial time series

## Feature Engineering
The following technical indicators are computed from closing prices:
- Simple Moving Average (SMA 10, SMA 50)
- Exponential Moving Average (EMA 10, EMA 50)
- Volatility (rolling standard deviation)
- Relative Strength Index (RSI)
- Moving Average Convergence Divergence (MACD)

## Data Processing
- Historical stock prices are scaled using Min-Max normalization
- Data is split chronologically to preserve time-series order
- Target variable is the closing price

## Evaluation Metrics
Model performance is evaluated using:
- Root Mean Squared Error (RMSE)
- Mean Absolute Percentage Error (MAPE)

## Output
- Numerical evaluation metrics printed to console
- Line plots comparing actual vs predicted stock prices
- Separate visualizations for Random Forest and LSTM predictions

## Use Case
This project is suitable for academic learning, experimentation with financial time series, and comparison of machine learning vs deep learning approaches for stock price prediction.
