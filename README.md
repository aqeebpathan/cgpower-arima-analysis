# 📊 CGPOWER Stock Price Forecast using ARIMA

## 📌 Objective
This assignment aims to analyze and forecast the stock price of CG Power and Industrial Solutions Ltd (CGPOWER) using time series analysis techniques. The ARIMA (AutoRegressive Integrated Moving Average) model is used for forecasting future stock prices based on historical data.


## 📂 Dataset
- Source: Yahoo Finance (via Python yfinance library)
- Stock: CGPOWER (NSE)
- Duration: Last 1 year of daily closing prices



## 🔧 Methodology

### 1. Data Preprocessing
- Converted date column into datetime format
- Set date as index
- Checked and handled missing values using forward fill method
- Visualized closing price trend over time



### 2. Stationarity Check (ADF Test)
- Applied Augmented Dickey-Fuller (ADF) Test
- If data was non-stationary, differencing was applied


### 3. ACF & PACF Analysis
- ACF (AutoCorrelation Function) used to determine MA (q)
- PACF (Partial AutoCorrelation Function) used to determine AR (p)



### 4. ARIMA Model
- Selected ARIMA parameters (p, d, q)
- Fitted ARIMA model to the dataset
- Evaluated model summary


### 5. Forecasting
- Predicted next 30 days stock prices
- Compared forecast with historical data

---

## 📊 Visualizations

### 📈 Closing Price Trend
<img width="1024" height="547" alt="image" src="https://github.com/user-attachments/assets/17755e53-b44d-467b-9c45-37f0cab19a84" />  

---

### 📉 ACF and PACF Plots
<img width="568" height="435" alt="image" src="https://github.com/user-attachments/assets/663cee56-caeb-4a94-9028-15349f1a2660" />

---

### 🔮 Forecasted Prices (Next 30 Days)
<img width="986" height="528" alt="image" src="https://github.com/user-attachments/assets/a0798104-dc67-4372-beff-9f136176ced1" />


---

## 📈 Results & Observations

The closing price trend of CG Power and Industrial Solutions Ltd over the past one year shows a fluctuating pattern with periods of both growth and decline. Initially, the stock experienced moderate volatility, followed by a strong upward movement reaching a peak around September–October. After this peak, the price showed a gradual decline and a sharp drop around January, indicating high market volatility during that period.

However, the stock demonstrated a strong recovery after the dip, with prices rising again towards the end of the observed period. Overall, the stock exhibits a cyclical pattern with no consistent long-term linear trend, but a recent upward momentum is visible.

The ACF plot indicates that most autocorrelation values lie within the confidence interval except for a few initial lags, suggesting that the series becomes weakly stationary after differencing. This supports the suitability of using the ARIMA model for forecasting.

The ARIMA model was successfully applied to the time series data, capturing the underlying patterns reasonably well. The forecast for the next 30 days shows continued fluctuations with a slight upward bias, but also indicates potential short-term volatility. There is no indication of a sharp continuous rise or fall; instead, the model predicts moderate movements within a range.

In conclusion, the stock is expected to remain somewhat volatile in the short term with a mild upward tendency. However, due to the unpredictable nature of stock markets, these predictions should be interpreted cautiously.

---

## ⚠️ Limitations

- Stock market is highly volatile and affected by external factors
- ARIMA model only considers historical data
- News, economic conditions, and global events are not included

---

## 💻 Tools & Technologies Used

- Python
- Google Colab
- Pandas, NumPy
- Matplotlib
- Statsmodels
- yFinance

---

## 📁 Repository Contents

- Jupyter Notebook (.ipynb)
- Dataset (.csv)
- Output Screenshots (.png)
- README.md

---

## 🤖 AI Ethics & Responsible Usage Declaration

I hereby declare that:

- The dataset used in this assignment is properly cited and ethically sourced.
- I have analyzed potential biases present in the dataset and model.
- I have considered privacy implications related to the data used.
- I understand the responsible and ethical usage of the developed system/model.
- This work adheres to institutional guidelines on ethical AI practices.

---

### Dataset Details:
- Source: Yahoo Finance (accessed using yfinance Python library)
- Type of Data: Historical stock price time series data (daily closing prices)
- Contains Personal/Sensitive Data? (Yes/No): No  
- If Yes, describe anonymization steps: Not applicable

---

### Identified Bias (if any):
The dataset represents only historical stock prices and does not include external influencing factors such as economic conditions, company news, or global events. This may introduce bias in predictions as the ARIMA model relies purely on past price patterns and ignores real-world influences.

---

### Responsible Usage Statement:
The developed ARIMA model is intended solely for academic and educational purposes. The predictions generated should not be used for real-world financial decision-making or investment advice. Stock markets are highly volatile and influenced by multiple unpredictable factors, and this model does not guarantee accurate future performance.

---

### Student Details:
- Student Name: Mohmmed Aqeeb Pathan
- UIN: 242A003 
- Course: TE-AI&DS
- Date: -
- Signature: PMAJ.
---


