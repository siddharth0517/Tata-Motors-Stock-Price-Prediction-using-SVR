# Tata Motors Stock Price Prediction using Support Vector Regression (SVR)
## Table of Contents
+ Overview
+ Installation
+ Data
+ Feature Engineering
+ Modeling
+ Evaluation
+ Results
+ Visualization
+ Future Work
+ Contributing

# Overview
+ This project aims to predict the future stock prices of Tata Motors using historical stock data and technical indicators like moving averages. The model used for this task is Support Vector Regression (SVR), which is well-suited for predicting continuous values.

+ By leveraging historical stock data, we build an SVR model to make stock price predictions and compare model performance against actual stock prices. The project also includes feature engineering and data visualization to improve understanding and model performance.

# Installation
+ To run this project, ensure you have the following libraries installed:
+ pandas
+ numpy
+ matplotlib
+ sklearn
  
# Data
+ The historical stock data of Tata Motors is collected using Kaggle or You Can use yfinance API. It includes:

+ Open, High, Low, Close prices
+ Adjusted Close price (adjusted for dividends and stock splits)
+ Volume (number of shares traded)

# Feature Engineering
+ To improve model performance, the following features are created:

+ MA20: 20-day moving average
+ MA50: 50-day moving average
+ These features capture short-term and medium-term trends in the stock prices.

# Modeling
+ The machine learning model used is Support Vector Regression (SVR) with the Radial Basis Function (RBF) kernel. It is trained on the moving averages and adjusted closing prices to predict future stock prices.


# Initialize SVR model
+ svr_model = SVR(kernel='rbf', C=1000, gamma=0.1)
+ svr_model.fit(X_train, y_train)

# Evaluation
+ The model is evaluated using the following metrics:

+ **Mean Squared Error (MSE):** Measures the average of the squared differences between predicted and actual values.
+ **R² Score:** Represents how well the model fits the data.

# Results
+ The SVR model achieves competitive performance in predicting the stock prices for Tata Motors. The results are evaluated based on the performance metrics (MSE, R²), and predicted vs. actual prices are visualized for comparison.

# Visualization
+ The project includes visualizations of the actual vs predicted stock prices using Matplotlib.

![image](https://github.com/user-attachments/assets/4a87518d-f383-467b-bec9-488df1256784)

#  Future Work
+ Additional Features: Incorporate more technical indicators like RSI, MACD, or Bollinger Bands.
+ Compare Models: Try other models such as Random Forest, XGBoost, or LSTM to see how they compare to SVR.
+ Sentiment Analysis: Include sentiment analysis from news or social media to enhance prediction.

# Contributing
+ Contributions are welcome! Feel free to open a pull request if you have any suggestions or improvements.

