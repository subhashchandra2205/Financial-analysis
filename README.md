# 📈 Indian Stock Market Analysis & Portfolio Optimization

A Python-based financial data analysis project focused on studying the historical performance, risk, returns, and market behavior of selected Indian stocks. The project combines **stock data analysis, visualization, CAPM analysis, portfolio asset allocation, and sentiment analysis** to derive data-driven insights from financial market data.

---

## 📌 Project Overview

This project analyzes historical stock-market data for **10 major Indian companies** along with the **NIFTY 50 index** as a market benchmark.

Historical adjusted closing prices are collected using the `yfinance` library and processed using Python's data-analysis and visualization libraries.

The project covers:

* 📊 Historical stock price analysis
* 📈 Stock performance visualization
* 📉 Return and risk analysis
* 📐 Capital Asset Pricing Model (CAPM)
* ⚖️ Portfolio asset allocation
* 📰 Stock sentiment analysis
* 📊 Statistical and interactive visualizations

The historical data used in the analysis spans approximately **January 2012 to April 2023**.

---

## 🎯 Objectives

The main objectives of this project are:

1. Collect and analyze historical stock-market data.
2. Study the price movement of selected Indian stocks.
3. Compare individual stock performance with the NIFTY 50.
4. Analyze stock returns and risk.
5. Apply the **Capital Asset Pricing Model (CAPM)** to evaluate systematic risk and expected returns.
6. Analyze different portfolio asset allocation strategies.
7. Study stock-market sentiment using sentiment data.
8. Present financial insights through effective visualizations.

---

## 📊 Stocks & Market Index

The project analyzes the following **11 assets**:

| Company / Index           | Yahoo Finance Ticker |
| ------------------------- | -------------------- |
| Reliance Industries       | `RELIANCE.NS`        |
| Tata Consultancy Services | `TCS.NS`             |
| HDFC Bank                 | `HDFCBANK.NS`        |
| Bharti Airtel             | `BHARTIARTL.NS`      |
| ICICI Bank                | `ICICIBANK.NS`       |
| State Bank of India       | `SBIN.NS`            |
| Infosys                   | `INFY.NS`            |
| ITC                       | `ITC.NS`             |
| Adani Enterprises         | `ADANIENT.NS`        |
| Tata Motors               | `TATAMOTORS.NS`      |
| NIFTY 50                  | `^NSEI`              |

The **NIFTY 50** is used as the market benchmark for comparative analysis.

---

## 📅 Dataset

### Historical Market Data

The stock data is downloaded using Yahoo Finance through the `yfinance` library.

**Requested period:**

```text
Start Date: 2012-01-01
End Date:   2023-04-30
```

After removing missing observations, the analysis contains approximately:

```text
2,776 rows × 11 columns
```

The project primarily uses the **Adjusted Close** price for analysis.

### Data Processing

The workflow includes:

1. Downloading historical data.
2. Selecting adjusted closing prices.
3. Combining the assets into a single Pandas DataFrame.
4. Handling missing values using `dropna()`.
5. Preparing the data for further financial analysis.
6. Normalizing data where required for comparison and visualization.

---

# 📂 Project Structure

```text
Indian-Stock-Market-Analysis/
│
├── CAPM.ipynb
├── Portfolio_Assets_Allocation.ipynb
├── Stocks_Data_Analysis_and_Visualization.ipynb
├── stock_sentiment.csv
└── README.md
```

---

# 📓 Project Notebooks

## 1. 📊 Stock Data Analysis & Visualization

### `Stocks_Data_Analysis_and_Visualization.ipynb`

This notebook focuses on exploratory analysis and visualization of historical stock-market data.

### Main tasks

* Download historical stock data using `yfinance`
* Create a combined stock-price DataFrame
* Handle missing values
* Analyze historical price movements
* Normalize stock-price data
* Compare stock performance
* Generate multiple stock-price plots
* Visualize trends across different companies and the NIFTY 50

The notebook uses multiple visualizations to make comparison between the selected securities easier.

---

## 2. 📐 Capital Asset Pricing Model (CAPM)

### `CAPM.ipynb`

The CAPM notebook evaluates the relationship between the expected return of an asset and its systematic risk relative to the market.

The CAPM equation is:

```text
E(Rᵢ) = Rf + βᵢ [E(Rm) − Rf]
```

Where:

* `E(Rᵢ)` = Expected return of the stock
* `Rf` = Risk-free rate
* `βᵢ` = Beta of the stock
* `E(Rm)` = Expected market return

### CAPM helps analyze

* Systematic risk
* Market sensitivity
* Beta
* Expected return
* Risk-return relationship

The NIFTY 50 is used as the market reference for the analysis.

---

## 3. ⚖️ Portfolio Asset Allocation

### `Portfolio_Assets_Allocation.ipynb`

This notebook focuses on portfolio construction and asset allocation.

The analysis studies how allocating capital among different stocks affects the overall characteristics of a portfolio.

### Key areas

* Asset allocation
* Portfolio returns
* Portfolio risk
* Diversification
* Risk-return trade-off
* Comparison of different allocations

The objective is to understand how portfolio composition can influence investment performance and risk.

---

## 4. 📰 Stock Sentiment Analysis

### `stock_sentiment.csv`

The project also contains a stock sentiment dataset.

This dataset can be used to investigate market sentiment associated with stocks and explore the relationship between sentiment and financial-market behavior.

The sentiment component complements the quantitative stock-price analysis by adding a qualitative market perspective.

---

# 🛠️ Technologies Used

The project is developed using **Python and Jupyter Notebook**.

### Programming Language

* Python

### Data Analysis

* `Pandas`
* `NumPy`

### Financial Data

* `yFinance`

### Visualization

* `Matplotlib`
* `Seaborn`
* `Plotly`

### Statistical Analysis

* `SciPy`

---

## 📦 Libraries

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

# 🔬 Methodology

The overall workflow of the project is:

```text
              Historical Stock Data
                       │
                       ▼
              Data Collection
                 using yFinance
                       │
                       ▼
              Data Preprocessing
                       │
              ┌────────┴────────┐
              ▼                 ▼
       Missing Value         Normalization
         Handling
              │                 │
              └────────┬────────┘
                       ▼
             Exploratory Analysis
                       │
                       ▼
              Stock Visualization
                       │
             ┌─────────┼─────────┐
             ▼         ▼         ▼
          Returns     Risk      CAPM
             │         │         │
             └─────────┼─────────┘
                       ▼
              Portfolio Analysis
                       │
                       ▼
              Sentiment Analysis
                       │
                       ▼
              Financial Insights
```

---

# 📈 Visualizations

The project generates visualizations to study the historical behavior of the selected stocks.

Examples include:

* Individual stock price trends
* Comparative stock-price charts
* Normalized price comparisons
* Portfolio-related visualizations
* CAPM-related analysis
* Interactive Plotly visualizations

### Sample Stock Price Analysis

The project generates individual time-series plots for stocks such as:

* Reliance Industries
* TCS
* HDFC Bank
* Bharti Airtel
* ICICI Bank
* SBI
* Infosys
* ITC
* Adani Enterprises
* Tata Motors
* NIFTY 50

---

# 🚀 How to Run the Project

## 1. Clone the Repository

```bash
git clone <https://github.com/subhashchandra2205/Financial-analysis>
```

Navigate to the project directory:

```bash
cd Indian-Stock-Market-Analysis
```

## 2. Install Dependencies

```bash
pip install pandas numpy yfinance matplotlib seaborn scipy plotly jupyter
```

## 3. Start Jupyter Notebook

```bash
jupyter notebook
```

Open the notebooks from the Jupyter interface.

### Recommended order

```text
1. Stocks_Data_Analysis_and_Visualization.ipynb
2. CAPM.ipynb
3. Portfolio_Assets_Allocation.ipynb
```

The sentiment dataset can be used alongside the relevant analysis.

---

# 📊 Key Insights

The project provides a framework for understanding:

* Long-term stock-price movements
* Relative performance of major Indian companies
* Market benchmark performance
* Stock return behavior
* Investment risk
* Systematic market risk
* CAPM-based expected returns
* Portfolio diversification
* Asset allocation
* Market sentiment

---

# 🔮 Future Improvements

The project can be extended by adding:

* Real-time stock-market data
* Automated portfolio optimization
* Sharpe ratio analysis
* Sortino ratio analysis
* Value at Risk (VaR)
* Maximum drawdown analysis
* Efficient Frontier visualization
* Portfolio backtesting
* More advanced NLP-based sentiment analysis
* Interactive Streamlit dashboard
* Automated investment-performance reports
* Additional Indian and international market indices

---

# ⚠️ Disclaimer

This project is created for **educational and analytical purposes only**.

The analysis presented in this repository should not be considered financial advice or a recommendation to buy, hold, or sell any security.

Past performance does not guarantee future results.

---

## ⭐ Project Highlights

```text
✓ 10 Indian Stocks + NIFTY 50
✓ ~2,776 observations
✓ Historical data from 2012–2023
✓ Yahoo Finance data collection
✓ Stock price analysis
✓ Data preprocessing & normalization
✓ Financial data visualization
✓ CAPM analysis
✓ Portfolio asset allocation
✓ Stock sentiment analysis
✓ Python-based financial analytics
```

---

## 📜 License

This project is intended for educational purposes. You are free to explore and modify the code with appropriate attribution.
