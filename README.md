# TCS Stock Price Trend & Directional Prediction

An end-to-end Python data analytics and machine learning pipeline that predicts next-day stock price movement (Bullish/Bearish) for TCS using historical equity data and technical indicators.

## 📌 Features & Highlights
•⁠  ⁠*Data Ingestion*: Automated retrieval using ⁠ yfinance ⁠ API.
•⁠  ⁠*Feature Engineering*: Engineered 20-day MA, 50-day MA, 14-day RSI, and Daily Returns.
•⁠  ⁠*Preprocessing*: Missing value handling and feature standardization via ⁠ StandardScaler ⁠.
•⁠  ⁠*Validation*: Strict chronological split (⁠ shuffle=False ⁠, 80/20 ratio) to prevent data leakage in time-series forecasting.
•⁠  ⁠*Modeling*: Tree-based classification using ⁠ RandomForestClassifier ⁠.

## 🛠️ Tech Stack
•⁠  ⁠*Language*: Python
•⁠  ⁠*Libraries*: pandas, numpy, scikit-learn, yfinance

## 📈 Key Results
•⁠  ⁠Achieved a realistic baseline directional classification accuracy of *50%* on unseen chronological test data without data leakage.
-
