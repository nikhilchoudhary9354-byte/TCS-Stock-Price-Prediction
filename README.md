# TCS Stock Trend Analysis

A small project where I analyzed TCS (Tata Consultancy Services) stock data and built a basic ML model to predict if the price will go up or down the next day.

## What it does

- Downloads TCS stock data (TCS.NS) using yfinance
- Calculates daily price range, daily returns, and a 50-day moving average
- Finds "bullish days" where the closing price is above the 50-day MA
- Plots the closing price vs the 50-day MA
- Trains a Random Forest model to predict if the price goes up or down the next day, using Close price, 50-day MA, and Daily Return as inputs
- Checks the model's accuracy against a simple baseline (just guessing the more common outcome), and prints precision/recall too

## How to run

1. Clone this repo
2. Install the libraries:
   ```
   pip install yfinance pandas matplotlib scikit-learn
   ```
3. Open and run `TCS_Stock_Tred_analysis.ipynb` in Jupyter or Google Colab

## Sample Output

```
Model Accuracy: 65.12 %
Baseline Accuracy (always guessing majority class): 53.49 %
```

## Notes

- This predicts price direction (up/down), not the actual future price.
- Data is only about 1 year, so results can vary a lot and shouldn't be taken as final.
- I compared the model's accuracy to a baseline guess to see if it's actually learning something useful.

## Tech Used

Python, Pandas, Matplotlib, yfinance, scikit-learn (Random Forest)

## Author

Nikhil Choudhary
[LinkedIn](https://linkedin.com/in/nikhilchoudhary) | [GitHub](https://github.com/nikhilchoudhary9354-byte)
