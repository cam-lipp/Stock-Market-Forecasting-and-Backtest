# Stock Market Forecasting & Backtest Tool

A MATLAB-based interactive tool that forecasts stock market direction, visualizes technical indicators, and backtests trading strategies.  
It combines classic technical analysis with machine learning and statistical modeling, including an ensemble model for more robust predictions.

---

## 📸 Preview
![Forecast Chart Example](preview.png)  
*Example forecast chart with SMA, Bollinger Bands, RSI, and flip points.*

---

## ✨ Features
- **Data Fetching** — Pulls historical OHLCV data from [Stooq](https://stooq.com) (no API key required).
- **Technical Indicators** — SMA, EMA, RSI, Bollinger Bands, MACD, ATR.
- **Statistical Feature** — Kalman filter drift estimation.
- **Machine Learning** — Ridge regression and ensemble modeling.
- **Backtesting** — Walk-forward simulation with Sharpe ratio and maximum drawdown.
- **Interactive Controls** — Adjust forecast horizon, longevity, and data window directly in MATLAB Live Editor.

---

## 🛠 How It Works
1. **Feature Engineering**  
   - Creates input features from price data, technical indicators, volatility measures, and drift estimates.  
2. **Model Training**  
   - Fits multiple models (including ridge regression) and combines predictions via an ensemble method.  
3. **Forecasting**  
   - Recursively simulates future closing prices to the chosen horizon.  
4. **Backtesting**  
   - Runs walk-forward tests, generates equity curves, and calculates performance stats.

---

## 📊 Example Output
- **Chart**: Price history, indicators, forecast line, flip points labeled with dates.
- **Stats**: Sharpe ratio, Max Drawdown, % Correct Direction.
- **Backtest Equity Curve**: Shows cumulative performance over the historical period.

---

## 🚀 Getting Started
**Requirements:**
- MATLAB R2022b or later (may work on older versions but untested)
- Statistics and Machine Learning Toolbox (optional, core functions implemented manually)

**Usage:**
1. Open the `StockMarketDataAnalysis.mlx` file in MATLAB.
2. Set your controls at the top:
   - **Ticker**: e.g., `AAPL`
   - **Interval**: `"1d"`, `"1wk"`, or `"1mo"`
   - **Show Last N Days**: e.g., `180`
   - **Forecast Horizon**: `"1M"`, `"3M"`, `"6M"`, `"1Y"`, `"2Y"`
   - **Longevity**: `"Short"`, `"Medium"`, `"Long"`
3. Click **Run All**.
4. View forecast plots and backtest results.

---

## ⚠ Disclaimer
This project is for **educational purposes only** and is **not financial advice**.  
Trading in financial markets carries significant risk, and past performance does not guarantee future results.

---

## 📄 License
MIT License – see `LICENSE` file for details.

---

## 📬 Contact
Created by [Your Name] – [LinkedIn](https://www.linkedin.com/in/your-link) | [GitHub](https://github.com/your-username)
