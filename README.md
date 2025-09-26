# Volatility Forecasting with GARCH Models

This project implements **volatility forecasting** for financial time series using the **NIFTY 50 index** as a case study.  
It leverages econometric models such as **ARIMA** and **GARCH-family models (GARCH, EGARCH, GJR-GARCH)** to predict conditional variance, evaluate forecast accuracy, and assess implications for **risk management and trading strategies**.

---

## Project Overview
- **Objective**: Forecast volatility of stock returns to better understand financial risk and its implications for derivative pricing and portfolio management.  
- **Dataset**: NIFTY 50 daily price data (downloaded via `yfinance`).  
- **Techniques Used**:
  - Data collection & preprocessing
  - Log-returns calculation
  - Stationarity testing (ADF Test)
  - ARIMA modeling for mean
  - GARCH-family models for volatility
  - Forecast evaluation (RMSE, MAE, QLIKE)
  - Backtesting (VaR)

---

---

## Methodology
1. **Data Preprocessing**
   - Retrieved historical NIFTY 50 data with `yfinance`
   - Computed log-returns
   - Conducted ADF test for stationarity

2. **Model Building**
   - ARIMA for mean equation
   - GARCH(1,1), EGARCH, and GJR-GARCH for volatility dynamics

3. **Forecasting & Evaluation**
   - Generated rolling one-step-ahead forecasts
   - Evaluated accuracy with RMSE, MAE, and QLIKE metrics
   - Compared performance across GARCH variants

4. **Visualization**
   - Plotted returns, volatility clustering
   - Forecast vs realized volatility graphs
   - Value-at-Risk (VaR) backtest

---

## Results
- Volatility clustering clearly observed in NIFTY 50 returns.  
- GARCH(1,1) provided strong baseline forecasts.  
- EGARCH captured asymmetry in shocks (leverage effects).  
- Models evaluated with RMSE, MAE, and QLIKE showed [fill in your results here].  

---

## Tech Stack
- **Python**: pandas, numpy, matplotlib, seaborn  
- **Statsmodels**: ARIMA, statistical testing  
- **arch**: GARCH-family models  
- **yfinance**: Data collection  

---

## Future Work
- Incorporate multivariate GARCH models (DCC-GARCH)  
- Extend to intraday high-frequency data  
- Compare with machine learning volatility models (LSTM, XGBoost)  

---

## Author
**Karandeep Singh**  
B.Tech in Electrical Engineering, IIT Bombay  
Interest: Quantitative Finance | Trading | Data Science  


