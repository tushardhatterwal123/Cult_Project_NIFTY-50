# 📈 Data-Driven Investment Intelligence Using NIFTY-50 Market Data

## Overview

This project builds an AI-powered investment intelligence platform using historical NIFTY-50 stock market data. The system combines data analysis, machine learning, deep learning, portfolio optimization, risk assessment, and model explainability to generate actionable investment insights.

### Key Features

* Exploratory Data Analysis (EDA) on NIFTY-50 stocks
* Technical Indicator Engineering (SMA, EMA, RSI, MACD, Bollinger Bands, etc.)
* Stock Direction Prediction using XGBoost
* Stock Price Forecasting using LSTM Neural Networks
* Portfolio Optimization using Modern Portfolio Theory
* Risk Assessment and Performance Metrics
* Model Explainability using SHAP

---

## Environment Setup

### Prerequisites

* Python 3.9 or higher
* Jupyter Notebook / Google Colab
* Access to the NIFTY-50 dataset

### Clone the Repository

```bash
git clone <repository-url>
cd nifty50-investment-intelligence
```

---

## Dependency Installation

Install all required packages:

```bash
pip install pandas numpy matplotlib seaborn plotly
pip install scikit-learn xgboost
pip install tensorflow
pip install PyPortfolioOpt
pip install shap
pip install ta
pip install tqdm
```

Alternatively:

```bash
pip install -r requirements.txt
```

### Main Libraries Used

* pandas
* numpy
* matplotlib
* seaborn
* plotly
* scikit-learn
* xgboost
* tensorflow / keras
* PyPortfolioOpt
* shap
* ta
* tqdm

---

## Dataset

Dataset: **NIFTY-50 Stock Market Data**

Source:
https://www.kaggle.com/datasets/rohanrao/nifty50-stock-market-data

Expected structure:

```text
nifty-50/
│
├── metadata.csv
├── RELIANCE.csv
├── TCS.csv
├── INFY.csv
├── ...
└── other stock files
```

Update the dataset path in the notebook before execution.

---

## Running the Application

### Option 1: Google Colab

1. Upload the notebook.
2. Mount Google Drive.
3. Place the dataset folder in Drive.
4. Update:

```python
DATA_DIR = "/content/drive/MyDrive/nifty-50"
```

5. Run all notebook cells sequentially.

### Option 2: Local Jupyter Notebook

Launch Jupyter:

```bash
jupyter notebook
```

Open:

```text
NIFTY50_Project.ipynb
```

Update the dataset path:

```python
DATA_DIR = "path/to/nifty-50"
```

Run all cells from top to bottom.

---

## Reproducing Results

### Step 1: Load and Clean Data

* Load all stock CSV files.
* Merge into a master dataframe.
* Handle missing values and duplicates.

### Step 2: Perform EDA

* Market-wide price analysis
* Sector performance analysis
* Volatility analysis
* Correlation heatmaps

### Step 3: Feature Engineering

Generate technical indicators:

* SMA
* EMA
* RSI
* MACD
* Bollinger Bands
* Volatility measures

### Step 4: Train Prediction Models

#### XGBoost Classifier

Objective:

* Predict whether next-day stock price will move up or down.

Evaluation:

* Accuracy
* Precision
* Recall
* F1 Score

#### LSTM Forecasting Model

Objective:

* Forecast future stock prices.

Evaluation:

* MAE
* RMSE
* R² Score
* Directional Accuracy

### Step 5: Portfolio Optimization

Use PyPortfolioOpt to:

* Estimate expected returns
* Calculate covariance matrix
* Generate optimized portfolio weights

### Step 6: Risk Assessment

Compute:

* Volatility
* Sharpe Ratio
* Maximum Drawdown
* Value at Risk (VaR)

### Step 7: Model Explainability

Use SHAP to:

* Interpret XGBoost predictions
* Identify most influential technical indicators

---

## Project Structure

```text
.
├── NIFTY50_Project.ipynb
├── README.md
├── requirements.txt
└── dataset/
    ├── metadata.csv
    ├── stock CSV files
    └── ...
```

---

## Authors

* Tushar (23321031)
* Sumit Kulhari (23118075)


