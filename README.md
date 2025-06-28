# StockPricePredictionKNN

Oracle (ORCL) Stock Price Movement Predictor

This project uses historical stock data for Oracle (ORCL) to predict daily price direction (up or down) using a K-Nearest Neighbors (KNN) classification model. It includes data collection, feature engineering, model training, and visualization to demonstrate how machine learning can be applied to financial data.

Technologies Used
Python, pandas, NumPy, yfinance, scikit-learn, matplotlib, seaborn

Project Overview

Pulled approximately 40 years of historical stock data for Oracle (1986–2025) using the yfinance API.

Engineered features such as daily returns and binary labels to indicate whether the stock price increased or decreased.

Built a K-Nearest Neighbors (KNN) classifier using five technical indicators: Open, High, Low, Close, and Volume.

Normalized the data using StandardScaler and split it into training and testing sets using an 80:20 ratio.

Achieved a model accuracy of approximately 80–85% on test data.

Visualized predicted vs. actual stock price directions using matplotlib to interpret model performance.

Insights Gained

Applied financial concepts and machine learning techniques to real-world stock data.

Explored the importance of feature engineering and normalization in classification tasks.

Gained experience using evaluation metrics and visualization tools to assess model performance.

Potential Improvements

Add more technical indicators such as RSI or MACD.

Test alternative classification models like Logistic Regression, Random Forest, or XGBoost.

Implement backtesting and portfolio simulation for real-time strategy evaluation.

Author
Aastha Mirchandani
Finance & Computer Science | University of San Francisco
