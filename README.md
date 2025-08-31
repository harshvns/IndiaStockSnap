# India Stock Snap

A **multi-factor model** to predict Indian stock market opening prices using **global cues, macro assets, technical indicators, and news sentiment**.  

---

## 📌 Overview  

This project forecasts the **next-session open** for Indian indices/stocks by combining multiple signals:  

- **Macro Factors:** Gold, crude oil, USD/INR, DXY  
- **Global Lead–Lag:** Prior closes/overnights of US, EU, and Asia markets  
- **Technicals:** MA50/MA200, Bollinger Bands, volatility  
- **Sentiment:** News related to tariffs, geopolitics, demand/supply  

---

## 📊 Key Signals  

- **MA50 and MA200 percent distances:**  

- **Blended MA signal:**  
(with small, tunable weights)

- **Other Features:**  
- Gap-open and return-based features  
- Calendar/holiday flags  

---

## 🛠 Tech Stack  

- **Languages & Environment:** Python, Google Colab  
- **Libraries:** pandas, numpy, scikit-learn, TA-Lib/ta, matplotlib, seaborn  
- **APIs & Data Sources:**  
- Prices/FX/commodities: Yahoo Finance (yfinance), Alpha Vantage  
- News: NewsAPI, GDELT  

> ⚠️ Follow each provider’s **Terms of Service**  

---

## 🚀 Usage  

1. Open the notebook **`IndiaStockSnap.ipynb`** in Colab.  
2. Set tickers, date range, and API keys (if required).  
3. Run all cells to:  
 - Fetch market/macro/news data  
 - Engineer features  
 - Train models  
 - Predict the next open  
4. Tune MA weights (**w50, w200**) and evaluate using:  
 - MAE  
 - RMSE  
 - Directional hit rate  

---

## 🔮 Future Scope  

- Advanced sentiment models tuned for **finance and multilingual news**  
- Inclusion of more **India-specific macro factors** (CPI/WPI, PMI, RBI events)  
- Deployment via **Web/API** for daily live predictions  

---

## ⚠️ Disclaimer  

This project is for **research and educational purposes only**.  
It is **not investment advice**.  

**Developed as a college project.**  
