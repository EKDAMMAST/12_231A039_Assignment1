# 📊 Stock Price Forecasting using ARIMA (CSV Dataset)

---

## (1) Problem Statement

This project focuses on analyzing historical stock price data stored in a CSV file and forecasting future stock prices using time series modeling. The challenge is to process real-world financial data, ensure stationarity, and build an accurate forecasting model using ARIMA.

---

## (2) Objective

* To load and preprocess stock data from a CSV file
* To analyze trends and patterns in stock prices
* To apply ARIMA model for time series forecasting
* To predict the next 30 days of closing prices
* To visualize and interpret the forecasting results

---

## (3) Dataset

**Source:**
NSE Historical Data (Downloaded as CSV file)

**File Used:**
`Quote-Equity-ALKEM-EQ-21-03-2026-21-04-2026.csv`

**Features:**

* Date
* Open Price
* High Price
* Low Price
* Close Price
* Volume

**Size:**
Daily stock data for approximately 1 month

---

## (4) Methodology

### 🔹 Data Preprocessing

* Loaded CSV file using pandas
* Converted Date column to datetime format
* Sorted data in chronological order
* Handled missing values using forward fill
* Selected closing price for modeling

### 🔹 Exploratory Data Analysis (EDA)

* Plotted closing price trends
* Observed fluctuations and patterns
* Performed Augmented Dickey-Fuller (ADF) test for stationarity

### 🔹 Model Building

* Applied differencing to make data stationary
* Used ACF and PACF plots to determine ARIMA parameters
* Built ARIMA model using `statsmodels`

### 🔹 Evaluation

* Compared predicted vs actual values
* Analyzed residuals and model summary
* Checked trend consistency

---

## (5) Results

* Successfully implemented ARIMA model on CSV dataset
* Forecasted stock prices for the next 30 days
* Generated visualizations for historical and predicted values

**Insights:**

* Stock prices show short-term fluctuations
* ARIMA provides reliable short-term forecasts
* Model accuracy improves with proper parameter tuning

---

## (6) How to Run

```bash
pip install -r requirements.txt
python main.py
```

---

## (7) Conclusion

The project demonstrates how time series forecasting can be performed using ARIMA on stock price data stored in a CSV file. The model captures trends effectively and provides useful predictions for short-term analysis. However, real-world factors like market sentiment and news are not considered.

---

## (8) Student's Details

**Name:** Atharv Bhandare
**UIN No.:** 231A039
**Roll No.:** 12

---

## ⚖️ AI Ethics & Responsible Usage

* Data used is publicly available and does not violate privacy
* Model is built strictly for academic purposes
* Predictions should not be used for real financial decision-making

---
