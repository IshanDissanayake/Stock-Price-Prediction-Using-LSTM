# Stock-Price-Prediction-Using-LSTM
This project implements a Long Short-Term Memory (LSTM) neural network model to predict stock closing prices based on historical price data. The model is built using TensorFlow and is designed to forecast the stock market's future movements, helping with market analysis and decision-making. The project leverages several advanced techniques, including statistical analysis, feature engineering, and dynamic learning rate adjustments, to improve prediction accuracy.

## Overview
This repository demonstrates a time-series forecasting model that predicts stock closing prices using LSTM networks. The model is trained using historical stock price data and incorporates features such as the moving average, price volatility, and lagged stock prices. The approach combines statistical techniques for time series analysis with deep learning to provide a robust solution for stock price prediction.

## Technologies Used
* **Python 3.x**: Programming language used for the project.
* **TensorFlow**: Deep learning framework used for implementing the LSTM model.
* **yfinance**: Library for extracting stock price data from Yahoo Finance.
* **Statsmodels**: Used for statistical analysis and the Augmented Dickey-Fuller test (adfuller).
* **Matplotlib / Seaborn**: For data visualization (plots, graphs, etc.).
* **Keras**: For building and training the LSTM model.
* **Scikit-learn**: For additional machine learning utilities like scaling data.
* **ReduceLROnPlateau**: Used for dynamic learning rate adjustment to improve model performance during training.

## Data Collection
Stock price data is collected using the `yfinance` library, which pulls historical stock prices from Yahoo Finance. The dataset includes daily stock prices, with a focus on the 'Close' price, which is used as the target variable for prediction.

## Model Architecture
The LSTM model is a deep learning model that is particularly well-suited for time-series forecasting tasks. The architecture includes:

- LSTM layers to capture sequential dependencies in stock price movements.
- Dense layers to output the final prediction (stock closing price).
- Dropout layers to prevent overfitting.
  
The model is trained with dynamic learning rate adjustments using the ReduceLROnPlateau callback, which reduces the learning rate when the validation loss plateaus.

## Prerequisites
Make sure you have Python 3.x installed. You can install the required dependencies using `pip` or `conda`:

`pip install -r requirements.txt`

## License
This project is licensed under the MIT License - see the `LICENSE` file for details.
