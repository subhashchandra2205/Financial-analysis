# 📈 Stock Market Analysis, CAPM & Portfolio Optimization

A Python-based financial analysis project that studies historical stock-market data, evaluates stock performance and risk, applies the **Capital Asset Pricing Model (CAPM)**, analyzes portfolio asset allocation, and incorporates **stock sentiment analysis**.

---

## 📌 Project Overview

This project uses historical market data to analyze the performance and risk characteristics of selected Indian stocks and the NIFTY 50 index.

The project combines:

* 📊 Stock market data analysis
* 📈 Historical price visualization
* 💰 Return analysis
* ⚖️ Risk and volatility analysis
* 📐 CAPM analysis
* 🧮 Portfolio asset allocation
* 📰 Stock sentiment analysis
* 📉 Data visualization

Historical market data is obtained using **Yahoo Finance through the `yfinance` Python library**.

---

## 🎯 Objectives

The main objectives of this project are:

1. Analyze historical price movements of selected Indian stocks.
2. Compare the performance of different stocks against the NIFTY 50.
3. Calculate and analyze stock returns.
4. Study the risk and volatility associated with individual stocks.
5. Apply CAPM to estimate expected returns and systematic risk.
6. Analyze different portfolio asset allocation strategies.
7. Study stock-related sentiment and its potential relationship with market behavior.
8. Use visualizations to communicate financial insights effectively.

---

## 📂 Project Structure

```text
Stock-Market-Analysis/
│
├── CAPM.ipynb
│
├── Portfolio_Assets_Allocation.ipynb
│
├── Stocks_Data_Analysis_and_Visualization.ipynb
│
├── stock_sentiment.csv
│
└── README.md
```

---

## 📊 Stocks & Market Index Used

The analysis considers **11 assets**, including the NIFTY 50 benchmark.

| Asset                     | Ticker          |
| ------------------------- | --------------- |
| Reliance Industries       | `RELIANCE.NS`   |
| Tata Consultancy Services | `TCS.NS`        |
| HDFC Bank                 | `HDFCBANK.NS`   |
| Bharti Airtel             | `BHARTIARTL.NS` |
| ICICI Bank                | `ICICIBANK.NS`  |
| State Bank of India       | `SBIN.NS`       |
| Infosys                   | `INFY.NS`       |
| ITC                       | `ITC.NS`        |
| Adani Enterprises         | `ADANIENT.NS`   |
| Tata Motors               | `TATAMOTORS.NS` |
| NIFTY 50                  | `^NSEI`         |

### 📅 Data Period

**1 January 2012 – 30 April 2023**

The analysis uses the **Adjusted Close** price for the selected securities.

---

# 📁 Notebooks

## 1. 📊 Stock Data Analysis & Visualization

### `Stocks_Data_Analysis_and_Visualization.ipynb`

This notebook performs exploratory analysis of historical stock-market data.

### Key activities

* Download historical stock data
* Examine stock price movements
* Analyze adjusted closing prices
* Calculate returns
* Compare stock performance
* Analyze volatility
* Generate statistical insights
* Create visualizations for financial data

The notebook uses `yfinance` to retrieve historical market data and stores the downloaded data in Pandas DataFrames for further analysis.

---

## 2. 📐 Capital Asset Pricing Model

### `CAPM.ipynb`

This notebook applies the **Capital Asset Pricing Model (CAPM)** to analyze the relationship between risk and expected return.

CAPM is expressed as:

```text
E(Rᵢ) = Rf + βᵢ [E(Rm) − Rf]
```

Where:

* `E(Rᵢ)` = Expected return of the asset
* `Rf` = Risk-free rate
* `βᵢ` = Beta of the asset
* `E(Rm)` = Expected market return

The analysis can be used to understand how individual stocks behave relative to the broader market.

### Key concepts

* Market return
* Stock return
* Beta
* Systematic risk
* Expected return
* Risk-return relationship

---

## 3. ⚖️ Portfolio Asset Allocation

### `Portfolio_Assets_Allocation.ipynb`

This notebook focuses on constructing and evaluating portfolios using multiple assets.

The analysis examines the relationship between:

* Portfolio return
* Portfolio risk
* Asset weights
* Diversification
* Risk-return trade-off

Different asset allocations can be compared to understand how portfolio composition affects overall performance and risk.

---

## 4. 📰 Stock Sentiment Analysis

### `stock_sentiment.csv`

The project also includes a sentiment dataset containing stock-related information.

The dataset can be used to analyze market sentiment and investigate whether positive or negative sentiment is associated with changes in stock-market behavior.

---

# 🛠️ Technologies & Libraries

The project is developed using **Python** and Jupyter Notebook.

### Core libraries

```text
Python
Jupyter Notebook
Pandas
NumPy
yFinance
Matplotlib
Seaborn
SciPy
Plotly
```

### Library usage

| Library    | Purpose                            |
| ---------- | ---------------------------------- |
| Pandas     | Data manipulation and analysis     |
| NumPy      | Numerical calculations             |
| yFinance   | Downloading historical market data |
| Matplotlib | Data visualization                 |
| Seaborn    | Statistical visualization          |
| SciPy      | Statistical analysis               |
| Plotly     | Interactive visualizations         |

---

# 🚀 Getting Started

## Prerequisites

Make sure Python is installed on your system.

You can install the required libraries using:

```bash
pip install pandas numpy yfinance matplotlib seaborn scipy plotly jupyter
```

---

## ▶️ Running the Project

Clone the repository:

```bash
git clone <YOUR-GITHUB-REPOSITORY-URL>
```

Navigate to the project directory:

```bash
cd Stock-Market-Analysis
```

Start Jupyter Notebook:

```bash
jupyter notebook
```

Then open the required `.ipynb` file.

---

# 🔬 Methodology

The overall workflow of the project can be summarized as:

```text
Historical Market Data
        ↓
Data Collection using yFinance
        ↓
Data Cleaning & Preparation
        ↓
Exploratory Data Analysis
        ↓
Return & Risk Analysis
        ↓
CAPM Analysis
        ↓
Portfolio Asset Allocation
        ↓
Sentiment Analysis
        ↓
Visualization & Insights
```

---

# 📈 Expected Analysis

The project provides a framework for understanding:

* Historical stock price behavior
* Relative stock performance
* Investment returns
* Stock volatility
* Market-related systematic risk
* CAPM beta
* Expected returns
* Portfolio diversification
* Asset allocation
* Market sentiment

---

# 🔮 Future Improvements

Possible improvements to the project include:

* Add real-time market data
* Implement automated portfolio optimization
* Include Sharpe ratio and other risk-adjusted performance metrics
* Add Value at Risk (VaR) analysis
* Develop an interactive financial dashboard
* Improve sentiment analysis using NLP
* Compare multiple portfolio optimization techniques
* Add backtesting of portfolio strategies
* Automate the complete analysis pipeline

---

# ⚠️ Disclaimer

This project is intended for **educational and analytical purposes only**.

The analysis and results should not be considered financial advice or a recommendation to buy or sell any security.

---

# 👤 Author

**Subhash Chandra**

Mechanical Engineering
IIT Madras

---

## ⭐ Project Highlights

* Analysis of **11 Indian stocks/market assets**
* Historical data covering **2012–2023**
* Yahoo Finance data acquisition
* Stock return and risk analysis
* CAPM-based analysis
* Portfolio asset allocation
* Stock sentiment analysis
* Static and interactive financial visualizations
