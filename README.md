# 📈 Stock Market Prediction App

An AI-powered web application that analyzes historical stock data and predicts future stock prices using machine learning. The app is designed for educational and research purposes and is backed by a published research paper.

---

## 📖 Description

This project integrates machine learning and data visualization to forecast future stock trends. By using models like Linear Regression and LSTM, it learns from historical price movements and generates forward predictions.

The interface, built with Streamlit, allows users to enter a stock symbol, visualize past trends, and view predicted future prices. The model forecasts are plotted on an interactive graph that extends beyond the latest available real-time data.

> 🔍 **Note:** If you're unsure where prediction begins, observe the chart — the future dates (beyond today's data) and the change in curve style often represent forecasted values. You can further customize it with labels like "Actual" vs "Predicted" for clarity.

---

## 🎯 Objective

To predict stock prices for upcoming days using historical data and present those predictions interactively via a web app.

---

## 🔧 Technologies Used

- **Python** – Core programming language
- **Streamlit** – For building the web application
- **Scikit-learn** – Linear Regression and other ML models
- **TensorFlow / Keras** – LSTM model for time-series forecasting
- **Pandas & NumPy** – Data handling and preprocessing
- **Matplotlib & Plotly** – Data visualization
- **Yahoo Finance API (yfinance)** – Fetching historical stock data

---

## ✨ Features

- 🔍 Input a stock ticker and fetch real-time historical data
- 📉 Visualize stock trends interactively
- 🤖 Predict future stock prices using trained models
- 📆 Graph with extended future timeline based on predictions
- 📄 Supported with a **published research paper**

---

## 🚀 How to Run

1. **Clone or extract** the project files.
2. Open the folder in your preferred IDE (e.g., **VS Code**).
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
4. Run the Streamlit app:
      ```bash
     streamlit run app.py
     ```
5. The app will open in your browser. Enter a stock symbol (like AAPL or TSLA) to begin.

---

## 📈 How It Predicts

- The model takes past N days of stock prices to predict the next day's price.
- This is repeated to forecast several future days (multi-step prediction).
- Predictions are shown on the graph alongside historical data.
- The future prediction line starts from the most recent actual date and extends forward.
> 🧠 Behind the scenes: The LSTM or regression model is trained on historical sequences (like sliding windows) and outputs price forecasts, which are visualized in real-time.

---

## 🔮 Future Enhancements

- Add evaluation metrics like RMSE and MAE
- Support user authentication and watchlist
- Display news sentiment for stock impact analysis
- Save/export prediction reports as PDFs
- Deploy the app to the cloud for public access

