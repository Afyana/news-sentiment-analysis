# Financial News Sentiment Analysis

## Predicting Price Moves with News Sentiment

[![Python CI](https://github.com/Afyan/news-sentiment-analysis/actions/workflows/unittests.yml/badge.svg)](https://github.com/Afyan/news-sentiment-analysis/actions/workflows/unittests.yml)
[![Python Version](https://img.shields.io/badge/python-3.10%2B-blue)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

---

## 📋 Project Overview

This project is part of the **10 Academy - Artificial Intelligence Mastery** program (Week 1 Challenge). The objective is to build a rigorous analytical pipeline that:

1. **Quantifies sentiment** expressed in financial news headlines using NLP techniques
2. **Computes technical indicators** from historical stock price data
3. **Measures statistical relationships** between news sentiment and stock price movements
4. **Provides actionable investment strategies** based on findings

### Business Context

As a Data Analyst at **Nova Financial Solutions**, the goal is to separate signal from noise in financial news, enabling investment teams to leverage sentiment as a predictive tool for stock market trends.

---

## 📊 Dataset Description

### FNSPID (Financial News and Stock Price Integration Dataset)

| Field | Description |
|-------|-------------|
| headline | Article release headline |
| url | Direct link to full article |
| publisher | Author or creator |
| date | Publication date and time (UTC-4) |
| stock | Stock ticker symbol (e.g., AAPL) |

### Historical Stock Price Data (YFinance)

| Field | Description |
|-------|-------------|
| Date | Trading day timestamp |
| Open | Price at market open |
| High | Highest price of the day |
| Low | Lowest price of the day |
| Close | Price at market close |
| Adj Close | Adjusted closing price |
| Volume | Total shares traded |

### Stocks Analyzed

| Symbol | Company |
|--------|---------|
| AAPL | Apple Inc. |
| AMZN | Amazon.com Inc. |
| GOOG | Alphabet Inc. |
| META | Meta Platforms Inc. |
| NVDA | NVIDIA Corporation |

---

## 🎯 Learning Outcomes

### Skills Developed

- ✅ Environment setup with GitHub integration and CI/CD pipelines
- ✅ Exploratory Data Analysis on text and time series data
- ✅ NLP & Sentiment Analysis using VADER, TextBlob
- ✅ Technical indicators with TA-Lib and pandas_ta
- ✅ Statistical analysis with Pearson correlation
- ✅ Data visualization with Matplotlib and Seaborn

### Tools & Technologies

| Category | Technologies |
|----------|--------------|
| **Data Manipulation** | Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn |
| **NLP & Text Analysis** | NLTK, TextBlob, Scikit-learn |
| **Technical Indicators** | TA-Lib, pandas_ta |
| **Version Control** | Git, GitHub |
| **CI/CD** | GitHub Actions |
| **Environment** | Python 3.10+, VS Code |

---

## 📁 Project Structure
news-sentiment-analysis/
├── .github/workflows/
│   └── unittests.yml
├── data/
│   ├── raw/
│   │   ├── yfinance_data/
│   │   │   ├── AAPL.csv
│   │   │   ├── AMZN.csv
│   │   │   ├── GOOG.csv
│   │   │   ├── META.csv
│   │   │   └── NVDA.csv
│   │   └── raw_analyst_rating.csv
│   └── processed_news.csv
├── notebooks/
│   ├── 01_eda_analysis.ipynb
│   └── 02_technical_indicators.ipynb
├── src/
├── tests/
├── requirements.txt
├── .gitignore
└── README.md


## 🚀 Getting Started

### Prerequisites

- Python 3.10 or higher
- Git
- VS Code (recommended) or any Python IDE

### Installation

1. **Clone the repository**

```bash
git clone https://github.com/Afyan/news-sentiment-analysis.git
cd news-sentiment-analysis

python -m venv venv
venv\Scripts\activate

pip install -r requirements.txt

# Using conda (recommended for Windows)
conda install -c conda-forge ta-lib

# Using pip (may need pre-built wheels)
pip install TA-Lib

# News data
data/raw/raw_analyst_rating.csv

# Stock price data
data/raw/yfinance_data/AAPL.csv
data/raw/yfinance_data/AMZN.csv
data/raw/yfinance_data/GOOG.csv
data/raw/yfinance_data/META.csv
data/raw/yfinance_data/NVDA.csv
