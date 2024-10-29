# Stock Price Prediction

This repository contains a series of Jupyter Notebooks focused on predicting stock prices using various statistical and machine learning models. The project explores different approaches such as Moving Average, ARIMA, and LSTM models to forecast future stock prices based on historical data.

## Table of Contents
- [Project Overview](#project-overview)
- [Models Used](#models-used)
  - [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
  - [Moving Average](#moving-average)
  - [ARIMA](#arima)
  - [LSTM](#lstm)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)

## Project Overview

The aim of this project is to use time series analysis techniques and machine learning algorithms to predict stock prices. It starts with an exploratory data analysis (EDA) to understand the data, followed by implementing different prediction models:

1. **Moving Average**: A simple but effective method for smoothing stock price data.
2. **ARIMA**: A powerful statistical model for forecasting time series data.
3. **LSTM**: A recurrent neural network capable of learning long-term dependencies for sequential data.

## Models Used

### Exploratory Data Analysis (EDA)
The first step in the project involves understanding the dataset, which includes analyzing patterns, trends, and relationships in the stock price data. The notebook `EDA.ipynb` covers:
- Time series visualization
- Rolling statistics
- Data cleaning

### Moving Average
The `MovingAvg.ipynb` notebook covers the implementation of the **Moving Average** method. This method smooths out short-term fluctuations and highlights long-term trends in stock price data.

### ARIMA
In `ARIMA.ipynb`, we implement the **ARIMA (AutoRegressive Integrated Moving Average)** model, which combines autoregression, differencing, and moving averages to make predictions. This notebook includes:
- Parameter selection using ACF and PACF
- Model training and evaluation
- Forecasting future prices

### LSTM
`LSTM.ipynb` focuses on **Long Short-Term Memory (LSTM)**, a type of recurrent neural network. This model is designed to capture the sequential dependencies in time series data and is particularly suited for predicting stock prices.

## Installation

To run this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/Luv-valecha/Stock_Price_Prediction.git
   cd Stock_Price_Prediction

2. Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`

3. Install the required packages
   ```bash
   pip install -r requirements.txt

## Usage

1. Load your stock price dataset into the notebooks.
2. Run the notebooks in the following order:
-EDA.ipynb for exploratory data analysis
-MovingAvg.ipynb for Moving Average prediction
-ARIMA.ipynb for ARIMA model
-LSTM.ipynb for LSTM neural network
3. Adjust hyperparameters and retrain the models as needed to improve prediction accuracy.

## Results

1. Moving Average provides a smooth curve and is useful for identifying trends.
2. ARIMA performs well for linear time series data, capturing seasonality and trends.
3. LSTM excels in learning long-term dependencies and non-linear patterns, often outperforming statistical models for stock price prediction.

## Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page if you have any questions or suggestions.