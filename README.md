**India Stock Snap**

Multi-factor model to predict Indian stock market opening prices using global cues, macro assets, technicals, and news sentiment.

**Overview**

Forecast next-session open for Indian indices/stocks by combining:

Macro: gold, crude oil, USD/INR, DXY
Global lead–lag: prior closes/overnights of US/EU/Asia markets
Technicals: MA50/MA200, Bollinger Bands, volatility
Sentiment: news on tariffs, geopolitics, demand/supply

**Key Signals**

MA50 and MA200 percent distances: (Close − MA) / MA
Blended MA signal: w50pct_50 + w200pct_200 (small, tunable weights)
Gap-open and return-based features, calendar/holiday flags

**Tech Stack**

Python, Google Colab
pandas, numpy, scikit-learn, ta/TA-Lib, matplotlib/seaborn
yfinance/Alpha Vantage, NewsAPI/GDELT (optional)
Data Sources
Prices/FX/commodities: Yahoo Finance (yfinance), Alpha Vantage
News: NewsAPI, GDELT
Note: Follow each provider’s Terms of Service

**Usage**

Open the notebook (IndiaStockSnap.ipynb) in Colab
Set tickers, date range, and any API keys
Run all cells to fetch data, engineer features, train models, and predict next open
Tune MA weights (w50, w200) and evaluate (MAE, RMSE, directional hit rate)

**Future Scope**

Finance-tuned sentiment, multilingual news
More India-specific macro (CPI/WPI, PMI, RBI events)
Web/API for daily live predictions

Disclaimer: Research/education only, not investment advice.
Developed as a college project
