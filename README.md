# 📈 Oracle Stock Price Movement Predictor

A machine learning project that predicts the daily price movement of **Oracle (ORCL)** stock using a **K-Nearest Neighbors (KNN)** classification model. By leveraging nearly 40 years of historical market data, the project demonstrates how machine learning techniques can be applied to financial forecasting through data preprocessing, feature engineering, model training, and visualization.

---

## Table of Contents

1. Features
2. How It Works
3. Why It Matters
4. Tech Stack
5. Installation
6. Usage
7. Project Structure
8. Results
9. Future Improvements
10. Contributors

---

# Features

- **Historical Market Data**
  - Retrieved approximately **40 years** of Oracle (ORCL) stock data (1986–2025) using the **yfinance API**
  - Collected daily Open, High, Low, Close, and Volume data

- **Feature Engineering**
  - Calculated daily returns
  - Created binary labels indicating whether the stock price increased or decreased
  - Selected five key technical indicators for prediction

- **Machine Learning Model**
  - Built a **K-Nearest Neighbors (KNN)** classifier
  - Standardized features using **StandardScaler**
  - Split the dataset into **80% training** and **20% testing**

- **Performance Evaluation**
  - Achieved **80–85% classification accuracy**
  - Compared predicted versus actual stock price movements
  - Visualized model performance using charts

---

# How It Works

1. **Collect Historical Data**
   - Download Oracle stock data using the yfinance API.

2. **Prepare the Dataset**
   - Clean the data
   - Generate daily returns
   - Create binary target labels (Up or Down)

3. **Preprocess Features**
   - Normalize numerical features using StandardScaler.
   - Split data into training and testing sets.

4. **Train the Model**
   - Build and train a K-Nearest Neighbors classifier.

5. **Evaluate Performance**
   - Measure classification accuracy.
   - Visualize predicted versus actual stock movements.

---

# Why It Matters

Predicting stock price direction is an important challenge in quantitative finance.

This project demonstrates how machine learning can:

- Identify patterns in historical financial data
- Support investment decision-making
- Improve understanding of financial time series
- Showcase practical applications of predictive analytics in finance

---

# Tech Stack

### Programming Language

- Python

### Libraries

- pandas
- NumPy
- yfinance
- Scikit-learn
- Matplotlib
- Seaborn

### Machine Learning

- K-Nearest Neighbors (KNN)
- StandardScaler

### Development Tools

- Jupyter Notebook
- Git
- GitHub

---

# Installation

Clone the repository

```bash
git clone https://github.com/armirchandani/StockPricePredictionKNN.git
cd StockPricePredictionKNN
```

Install dependencies

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook StockPricePredictionKNN.ipynb
```

---

# Usage

### Download Historical Stock Data

```python
import yfinance as yf

stock = yf.download("ORCL", start="1986-01-01", end="2025-01-01")
```

### Train the KNN Model

```python
from sklearn.neighbors import KNeighborsClassifier

model = KNeighborsClassifier(n_neighbors=5)
model.fit(X_train, y_train)
```

### Evaluate Performance

```python
predictions = model.predict(X_test)
```

---

# Project Structure

```
StockPricePredictionKNN/
│
├── StockPricePredictionKNN.ipynb
├── README.md
└── requirements.txt
```

---

# Results

📈 Predicted Oracle stock price direction using historical market data

📊 Achieved approximately **80–85% classification accuracy**

⚙️ Successfully applied feature engineering and data normalization to improve model performance

📉 Visualized predicted versus actual stock movements to evaluate model effectiveness

---

# Future Improvements

- Incorporate additional technical indicators such as RSI, MACD, and Bollinger Bands
- Compare performance with Logistic Regression, Random Forest, and XGBoost
- Perform hyperparameter tuning using GridSearchCV
- Implement backtesting for trading strategy evaluation
- Build an interactive dashboard using Streamlit
- Explore deep learning models such as LSTMs for time-series forecasting

---

# Contributors

**Aastha Mirchandani**

Business Analytics Student | University of San Francisco

Interested in Machine Learning, Financial Analytics, Data Science, and FinTech

---

⭐ If you found this project helpful, consider giving it a star!
