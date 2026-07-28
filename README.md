# Time Series Forecasting of NHS Emergency Department Demand
A time series forecasting project that predicts **28-day paediatric emergency department attendances** for an NHS Acute Trust hospital using Facebook Prophet and benchmark forecasting methods.

## 📌 Project Overview
Accurate forecasting of emergency department attendances helps hospitals optimize staffing, improve patient flow, and allocate healthcare resources efficiently.
This project develops and evaluates forecasting models to predict daily paediatric emergency attendances over a 28-day horizon using three years of historical NHS data.

---

## 📊 Dataset

- **Observations:** 1,056 daily records
- **Period:** April 2014 – February 2017
- **Forecast Horizon:** 28 days
- **Target Variable:** Daily paediatric emergency attendances

---

## 🛠 Tech Stack

- Python
- Pandas
- Matplotlib
- Seaborn
- Prophet
- Statsmodels
- Forecast Tools

---

## 🔍 Exploratory Data Analysis

Key findings include:

- Peak emergency attendances occurred in **2016**
- **Weekends** experienced higher attendances than weekdays
- **March** recorded the highest monthly attendances
- **August** had the lowest attendances
- Strong weekly and yearly seasonal patterns were identified

---

## 📈 Forecasting Models

Models evaluated:

- Seasonal Naive (Benchmark)
- Prophet
- Prophet + UK Public Holidays ✅

Model evaluation used:

- Rolling Origin Cross Validation
- Mean Absolute Error (MAE)
- Mean Absolute Percentage Error (MAPE)
- Prediction Interval Coverage (PIC)
- Winkler Score

---

## 🏆 Best Model

**Prophet with UK Public Holidays**

The selected model outperformed the seasonal naive benchmark by achieving:

- Lower MAE
- Lower MAPE
- Better calibrated prediction intervals
- Improved forecast reliability across the 28-day horizon

---

## 📊 Key Insights

- Emergency attendances show clear weekly and yearly seasonality.
- Sundays are consistently the busiest days.
- March has the highest expected demand.
- Public holidays significantly influence emergency attendances.
- Forecasts indicate increasing demand from late February into March.

---

## 💡 Business Impact

The forecasting model supports:

- Medical workforce planning
- Emergency department staffing
- Resource allocation
- Patient flow management
- Reduction of staff burnout through better scheduling

---

## 📦 Project Workflow

- Data preprocessing
- Exploratory Data Analysis
- Time series feature extraction
- Baseline forecasting
- Prophet model development
- Cross-validation
- Forecast evaluation
- 28-day demand forecasting

---

## 📈 Results

✅ Prophet outperformed the seasonal naive benchmark.

✅ Captured long-term trends, weekly seasonality, yearly seasonality, and holiday effects.

✅ Produced reliable short-term forecasts suitable for operational planning in healthcare.

---

## 🚀 Future Improvements

- Incorporate weather data
- Include seasonal illness indicators
- Compare with ARIMA, SARIMA, LSTM, and Temporal Fusion Transformer (TFT) models
- Deploy as an interactive forecasting dashboard
