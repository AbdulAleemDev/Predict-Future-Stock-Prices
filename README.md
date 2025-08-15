# Task 2: Predict Future Stock Prices (Short-Term)

## 📌 Objective
The goal of this project is to use historical stock data to **predict the next day's closing price** for a selected stock.  
This involves:
- Loading market data from Yahoo Finance.
- Using features such as `Open`, `High`, `Low`, and `Volume`.
- Training a machine learning model to forecast the next `Close` value.

---

## 📊 Dataset
- **Source**: Yahoo Finance (retrieved via the [`yfinance`](https://pypi.org/project/yfinance/) Python library).
- **Ticker**: Example used — Apple (`AAPL`) *(can be replaced with Tesla `TSLA` or any other stock)*.
- **Date Range**: Last 1 year of trading data.
- **Features Used**:
  - `Open`
  - `High`
  - `Low`
  - `Volume`
- **Target**:
  - Next day's `Close` price.

---

## 🤖 Models Applied
Two approaches were implemented:
1. **Linear Regression**
   - Simple baseline model for price prediction.
2. **Random Forest Regressor**
   - Ensemble-based model for better handling of non-linear patterns.

---

## 📈 Key Results & Findings
- **Linear Regression**:
  - Captured general trends but struggled with volatile days.
- **Random Forest**:
  - Outperformed linear regression with **lower error** and better fit to sudden market changes.
- **Visual Analysis**:
  - Plotted **Actual vs Predicted Closing Prices**, showing that the Random Forest model tracked market movement more closely.

---

## 📷 Sample Plot
*(Example plot of Actual vs Predicted closing prices)*  
![Stock Price Prediction Plot](plot.png)

---

## 🚀 Future Improvements
- Experiment with deep learning models (e.g., LSTMs).
- Incorporate technical indicators (e.g., Moving Averages, RSI).
- Use longer historical windows for better trend learning.
