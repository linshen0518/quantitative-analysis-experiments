# 📊 Quantitative Analysis Experiments

This repository collects applied econometrics and quantitative analysis experiments in finance.  
Focus is on **statistical modeling and diagnostics**, not trading strategy backtests.  
財務計量分析與經濟計量模型實驗，包含多元迴歸、殘差診斷與時間序列建模。

---

## 1. Multiple Regression: BA & AAPL vs DJI
- **Question**: Can Boeing (BA) and Apple (AAPL) explain the variation of the Dow Jones Industrial Average (DJI)?
- **Methods**:  
  - OLS on log-levels  
  - OLS on log-returns with Newey–West robust errors  
  - Residual diagnostics (heteroskedasticity, autocorrelation, Q-Q plots)  
  - Multicollinearity check (VIF)  

👉 Notebook: [BA_AAPL_DJI_regression.ipynb](./BA_AAPL_DJI_regression-checkpoint.ipynb)

### Key Results
- Log-level OLS: R² ≈ **0.962**；BA≈0.157，AAPL≈0.336  
- Returns + HAC: R² ≈ **0.651**，DW≈2.15  
- Breusch–Pagan: heteroskedasticity present (handled with HAC)  
- VIF ≈ 1 → no multicollinearity issue  

---

## ⚙️ Tech stack
- Python (pandas, numpy, statsmodels, matplotlib, scipy, yfinance)

---

## 📌 Notes
This repository is for academic and research demonstration only.  
All analyses are based on **publicly available data** (Yahoo Finance).
