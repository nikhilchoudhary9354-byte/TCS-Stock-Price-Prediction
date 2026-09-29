# TCS Stock Trend Analysis

A Python project that analyzes TCS (Tata Consultancy Services) stock price data and builds a simple machine learning model to predict whether the stock price will go up or down the next day.

## What it does

- Downloads historical TCS stock price data (TCS.NS) using `yfinance`
- Calculates daily price range, daily returns, and a 50-day Moving Average
- Identifies "bullish days" (days when Close price is above the 50-day MA)
- Plots Close Price vs 50-day Moving Average over time
- Builds a Random Forest Classifier to predict next-day price direction (up/down), using Close price, 50-day MA, and Daily Return as features
- Compares model accuracy against a baseline (always guessing the majority class), and prints a full classification report (precision, recall, f1-score)

## How to run

1. Clone this repo
2. Install the required libraries:
   ```
   pip install yfinance pandas matplotlib scikit-learn
   ```
3. Run the notebook (`TCS_Stock_Tred_analysis.ipynb`) in Jupyter or Google Colab

## Sample Output

```
Model Accuracy: 65.12 %
Baseline Accuracy (always guessing majority class): 53.49 %
```

## Notes

- This is a classification model predicting price **direction** (up/down), not a time-series forecasting model predicting actual future prices.
- Dataset covers about 1 year of trading data, so results should be read with some caution given the limited sample size.
- Model accuracy is compared against a baseline to check whether it's actually better than just guessing the majority class.

## Tech Used

Python, Pandas, Matplotlib, yfinance, scikit-learn (Random Forest Classifier)

## Author

Nikhil Choudhary
[LinkedIn](https://linkedin.com/in/nikhilchoudhary) | [GitHub](https://github.com/nikhilchoudhary9354-byte)
