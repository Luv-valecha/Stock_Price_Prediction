# Stock Price Prediction Using ARIMA, LSTM, and Moving Averages

### Authors:
- Luv Valecha
- Dheeraj Kumar
- Dhruv Sharma
- Arafat Ahmed Sheikh

---

## Overview
This project aims to predict the future stock prices using previous data and models like ARIMA, LSTM, and Moving Averages. Each model has unique strengths to address time-series forecasting challenges in stock price prediction.

- **ARIMA (AutoRegressive Integrated Moving Average)**: A statistical model suitable for capturing historical stock price patterns by analyzing autocorrelations in the time series. Ideal for stationary data and short-term predictions by considering past values and error terms.

- **LSTM (Long Short-Term Memory)**: A type of recurrent neural network that captures long-term dependencies in sequential data. LSTM models handle complex non-linear patterns, predicting future prices based on historical trends and seasonality.

- **Moving Averages**: Smooth stock prices by removing noise and highlighting trends. The Simple Moving Average (SMA) and Exponential Moving Average (EMA) reveal short- and long-term trends, useful for strategy development.

---

## ARIMA Model for Stock Price Prediction

### Model
The ARIMA model combines three components:
1. **AR (AutoRegression)**: Uses the relationship between an observation and several lagged observations.
2. **I (Integrated)**: Differencing data makes it stationary, ensuring consistency over time.
3. **MA (Moving Average)**: Utilizes the dependency between observations and residual error terms from a moving average model on lagged errors.

**Parameterization**: ARIMA is expressed as ARIMA(p, d, q):
- `p`: Order of autoregressive part (number of lag observations).
- `d`: Degree of differencing (to make data stationary).
- `q`: Order of moving average part (number of lagged forecast errors).

### Model Implementation
To use ARIMA:
1. Make data stationary through differencing as needed.
2. Determine parameters `p` and `q` via ACF (Autocorrelation Function) and PACF (Partial Autocorrelation Function) plots.
3. Fit the model and evaluate its performance on historical data.

---

## LSTM Model for Stock Price Prediction

### Model
Long Short-Term Memory (LSTM) networks are advanced RNNs that model temporal sequences and capture long-term dependencies effectively.

#### Key Components:
1. **Forget Gate**: Decides which cell state information to discard.
2. **Input Gate**: Determines which new information to store in the cell state.
3. **Output Gate**: Controls the output from the cell state.

The combination of these gates allows LSTMs to retain or discard information selectively, making them suitable for time-series forecasting tasks, such as stock price prediction.

---

## Moving Averages for Stock Price Prediction

### Moving Averages
Moving Averages smooth price data and identify trends. There are two main types:
1. **Simple Moving Average (SMA)**: Averages a set number of past prices, such as a 10-day SMA.
2. **Exponential Moving Average (EMA)**: Assigns more weight to recent prices, making it more responsive to new information.

**Applications**: Moving averages help distinguish trends (upward, downward, sideways) and establish support/resistance levels. Crossovers between short- and long-term moving averages provide trading signals.

---

## Exploratory Data Analysis

1. **Time Series of Stock Prices (Open, High, Low, Adjusted Close)**:
   - **Observation**: Upward trend with some visible volatility.
   - **Inference**: Indicates Apple’s stock appreciation over time, with occasional volatility due to market events or economic factors.

2. **Moving Average for High Prices (10, 20, 30-day)**:
   - **Observation**: 10-day average captures short-term changes; 20- and 30-day averages show smoother trends.
   - **Inference**: Shorter averages capture recent changes, while longer averages highlight long-term trends.

3. **Volume Analysis**:
   - **Observation**: Spikes in trading volume at specific times.
   - **Inference**: Likely corresponds to significant market events, indicating increased interest and possibly a price trend after the event.

---
