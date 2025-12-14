# Stock Price Prediction using Machine Learning

This project implements a stock price prediction system using both traditional machine learning and deep learning models. It uses historical stock market data along with technical indicators to predict future stock prices.

The models implemented are:
- Random Forest Regressor
- LSTM (Long Short-Term Memory) Neural Network

The project fetches stock data dynamically using Yahoo Finance.

---

## Features

- Fetches historical stock data using yfinance
- Computes common technical indicators:
  - Simple Moving Average (SMA)
  - Exponential Moving Average (EMA)
  - Volatility
  - RSI (Relative Strength Index)
  - MACD
- Data scaling using MinMaxScaler
- Time-series aware train-test split
- Random Forest regression model
- LSTM deep learning model using TensorFlow/Keras
- Evaluation using RMSE and MAPE
- Visualization of predicted vs actual stock prices

---

## Tech Stack

- Python
- NumPy
- Pandas
- Matplotlib
- scikit-learn
- TensorFlow / Keras
- yfinance

---

## Project Structure

.
├── main.py
├── README.md
└── requirements.txt

---

## Installation

1. Clone the repository

   git clone https://github.com/Pranav-Kumar14/stock-price-prediction.git
   cd stock-price-prediction

2. Install dependencies

   pip install -r requirements.txt

---

## requirements.txt

numpy  
pandas  
matplotlib  
yfinance  
scikit-learn  
tensorflow  

---

## Usage

Run the script:

   python main.py

You will be prompted to enter a stock ticker symbol.

Example:

   Enter stock ticker symbol (e.g., AAPL, TSLA): AAPL

The script will:
- Download historical data
- Train Random Forest and LSTM models
- Evaluate both models
- Plot actual vs predicted prices

---

## Models Used

### Random Forest Regressor
- Ensemble-based regression model
- Good baseline for tabular financial features
- Uses 200 estimators with controlled depth

### LSTM Neural Network
- Designed for sequential/time-series data
- Two LSTM layers with dropout and batch normalization
- Optimized using Adam optimizer

---

## Evaluation Metrics

- RMSE (Root Mean Squared Error)
- MAPE (Mean Absolute Percentage Error)

These metrics are printed for each model during execution.

---

## Notes

- Data is split chronologically (no shuffling)
- LSTM input is reshaped to 3D format
- Predictions are inverse-transformed to original price scale
- This project is intended for academic and learning purposes

---

## Disclaimer

This project is not financial advice.  
Stock market predictions are inherently uncertain.

---

## Author

Pranav Kumar 

