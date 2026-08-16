# 📈 Indian Stock Market Analysis & Portfolio Optimization

A Python-based financial analytics project studying the historical performance, risk, and return behavior of major Indian stocks — combining price analysis, CAPM, portfolio allocation, and sentiment analysis into a single data-driven workflow.

---

## 📌 Overview

This project analyzes historical price data for **10 major Indian companies** plus the **NIFTY 50 index** as a market benchmark, using data pulled via `yfinance` and processed with Pandas/NumPy.

It covers:

- 📊 Historical stock price analysis & visualization
- 📉 Return and risk analysis
- 📐 Capital Asset Pricing Model (CAPM)
- ⚖️ Portfolio asset allocation
- 📰 Stock sentiment analysis

**Data period:** January 2012 – April 2023 (~2,776 rows × 11 columns after cleaning)

---

## 📊 Assets Analyzed

| Company / Index | Ticker |
|---|---|
| Reliance Industries | `RELIANCE.NS` |
| Tata Consultancy Services | `TCS.NS` |
| HDFC Bank | `HDFCBANK.NS` |
| Bharti Airtel | `BHARTIARTL.NS` |
| ICICI Bank | `ICICIBANK.NS` |
| State Bank of India | `SBIN.NS` |
| Infosys | `INFY.NS` |
| ITC | `ITC.NS` |
| Adani Enterprises | `ADANIENT.NS` |
| Tata Motors | `TATAMOTORS.NS` |
| NIFTY 50 (benchmark) | `^NSEI` |

---

## 📂 Repository Structure

```text
Financial-analysis/
│
├── Stocks_Data_Analysis_and_Visualization.ipynb
├── CAPM.ipynb
├── Portfolio_Assets_Allocation.ipynb
├── stock_sentiment.csv
└── README.md
```

---

## 📓 Notebooks

### 1. Stock Data Analysis & Visualization
`Stocks_Data_Analysis_and_Visualization.ipynb`
Downloads historical adjusted close prices, builds a combined DataFrame, handles missing values, normalizes prices, and visualizes trends across all 11 assets.

### 2. Capital Asset Pricing Model (CAPM)
`CAPM.ipynb`
Applies the CAPM formula to estimate expected returns based on systematic risk (β) relative to the NIFTY 50:

```
E(Rᵢ) = Rf + βᵢ [E(Rm) − Rf]
```

### 3. Portfolio Asset Allocation
`Portfolio_Assets_Allocation.ipynb`
Explores how different capital allocations across stocks affect overall portfolio return, risk, and diversification.

### 4. Stock Sentiment Analysis
`stock_sentiment.csv`
Sentiment dataset used to add a qualitative layer alongside the quantitative price/return analysis.

---

## 🛠️ Tech Stack

- **Language:** Python (Jupyter Notebook)
- **Data:** `yfinance`
- **Analysis:** `pandas`, `numpy`, `scipy`
- **Visualization:** `matplotlib`, `seaborn`, `plotly`

```python
import pandas as pd
import yfinance as yf
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import plotly.express as px
import plotly.graph_objects as go
from scipy import stats
```

---

## 🚀 Getting Started

```bash
git clone https://github.com/subhashchandra2205/Financial-analysis
cd Financial-analysis
pip install pandas numpy yfinance matplotlib seaborn scipy plotly jupyter
jupyter notebook
```

Recommended notebook order:
1. `Stocks_Data_Analysis_and_Visualization.ipynb`
2. `CAPM.ipynb`
3. `Portfolio_Assets_Allocation.ipynb`

---

## 📊 Key Insights

- Comparative performance of 10 major Indian stocks vs. the NIFTY 50 benchmark
- Systematic risk (β) and CAPM-based expected returns per stock
- Portfolio-level risk/return trade-offs under different allocation strategies
- Market sentiment as a complementary signal to price-based analysis

---

## 🔮 Future Improvements

- Real-time data integration
- Automated portfolio optimization (Efficient Frontier)
- Sharpe / Sortino ratio and Value-at-Risk (VaR) analysis
- Maximum drawdown analysis & backtesting
- NLP-based sentiment analysis
- Interactive Streamlit dashboard

---

## ⚠️ Disclaimer

This project is for **educational and analytical purposes only**. It does not constitute financial advice or a recommendation to buy, hold, or sell any security. Past performance does not guarantee future results.
