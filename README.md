# 📊 Time Series Analysis and Forecasting For Stock Market

## 🔍 Project Overview
This project focuses on forecasting **Apple (AAPL) stock prices** using both classical statistical models (**ARIMA, SARIMA, Prophet**) and a deep learning model (**LSTM**).  
The work was carried out as part of a structured 12-week forecasting project, including **preprocessing, model building, evaluation, and visualization**.

The main goal is to **compare different forecasting approaches**, evaluate their performance using **MAE, RMSE, MAPE**, and explore future stock price predictions.

---

## 📂 Repository Structure
- ├── Models/
- │ ├── arima_model.ipynb
- │ ├── arima_predictions.csv
- │ ├── final_evaluation.csv
- │ ├── future_arima.csv
- │ ├── future_comparison.csv
- │ ├── future_evaluation.csv
- │ ├── future_lstm.csv
- │ ├── future_prophet.csv
- │ ├── future_sarima.csv
- │ ├── prophet_model.ipynb
- │ ├── prophet_predictions.csv
- │ ├── sarima_model.csv
- │ └── sarima_predictions.csv
- ├── AAPL_clean.csv # Preprocessed dataset
- ├── ARIMA_Future_Forecast.ipynb
- ├── code.pynb
- ├── CSV_Download.ipynb
- ├── evaluation_metrics_on_forecasting.ipynb
- ├── final_comparison.ipynb
- ├── final_evaluation.ipynb
- ├── future_comparison.ipynb
- ├── future_tuned.ipynb
- ├── lstm_forecasting.ipynb
- ├── performance_metrics.ipynb
- ├── Prophet_Future_Forecasting.ipynb
- ├── SARIMA_Future_Forecast.ipynb
- ├── TIME SERIES ANALYSIS AND FORECASTING FOR STOCK MARKET.pdf
- ├── Time series stock market_20250417_183146_0000 (1)
- └── README.md


---

## 📊 Dataset
- **Source:** [Yahoo Finance / Kaggle AAPL Dataset]  
- **Range:** 2015 – 2024 (approx. 2500+ business days)  
- **Feature Used:** Date, Close Price  

**Preprocessing steps:**
- Missing value handling  
- Date indexing & sorting  
- Scaling (for LSTM only)  
- Train-test split with rolling origin  

---

## ⚡ Models Implemented
- **ARIMA** – AutoRegressive Integrated Moving Average  
- **SARIMA** – Seasonal ARIMA with seasonal differencing  
- **Prophet** – Additive model with trend, seasonality & changepoints  
- **LSTM** – Deep learning Recurrent Neural Network for nonlinear dependencies  

---

## 📈 Results & Evaluation
- **Metrics:** MAE, RMSE, MAPE  
- **Residual diagnostics performed:** stationarity tests, white-noise checks  

**Key Findings:**
- **LSTM** performed best on **short-term forecasts**  
- **Prophet** provided **smoother long-term forecasts**  
- **ARIMA/SARIMA** captured short-term dynamics but struggled with rapid volatility  

---

## 🚀 How to Run
1. Clone the repo:
```
git clone https://github.com/your-username/stock-forecasting.git
cd stock-forecasting
```
2. Install Dependencies
```
pip install -r requirements.txt
```
3. Run notebooks in order:
   - preprocessing.ipynb
   - arima_sarima.ipynb
   - prophet.ipynb
   - lstm.ipynb
   - final_comparision.ipynb

---

## 📌 Future Work
- Add hybrid/ensemble models (stacked forecasts)
- Deploy via Streamlit/Flask web app
- Extend dataset to other tech stocks (MSTF, AMZN, TSLA, etc.)
- Integrate external features (macro indicators, sentiment analysis)

---

## 📝 License
This project is released under the MIT License.
