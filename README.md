# AdEase Time Series Forecasting

## 📌 Project Overview

AdEase is an advertising technology platform that helps businesses optimize ad placements by maximizing clicks at minimal cost. This project focuses on analyzing and forecasting daily Wikipedia page views to support data-driven ad placement strategies across different languages, regions, and access types.

The dataset contains 550 days of view data for 145k+ Wikipedia pages, making this a large-scale time series forecasting problem.

## 🎯 Objective

- Analyze historical page view trends

- Forecast future traffic to optimize ad placement

- Evaluate performance using MAPE (target: 4–8%)
## 📂 Dataset

- train_1.csv: Daily page views for Wikipedia pages

- Exog_Campaign_eng.csv: Campaign indicator (English pages only)

### Page name format:

`<Title>_<Language>.wikipedia.org_<Access Type>_<Access Origin>`


### Extracted features:

Title, Language, Access Type, Access Origin

## 🔍 Exploratory Data Analysis

- Data structure and missing value analysis

- Page name parsing and feature extraction

- Language-wise and device-wise traffic trends

- Visualization of trends and seasonality

## 🧪 Stationarity & Time Series Analysis

- Dickey-Fuller test

- Time series decomposition

- Log transformation and differencing

- ACF & PACF analysis

## 🤖 Models Implemented

- ARIMA: Baseline time series forecasting

- SARIMAX: Includes campaign data as an exogenous variable

- Facebook Prophet: Handles seasonality and trend changes

- Hyperparameter tuning performed using grid search for at least one model.

## 📊 Evaluation

- Metric: MAPE

- Achieved accuracy within 4–8%

- Comparison across languages and models

## 🔧 Pipeline

- Modular functions for:

  - Preprocessing
  
  - Stationarity checks
  
  - Modeling and forecasting
  
  - Scalable pipeline for multiple time series

## 🧠 Key Insights

- English pages show highest traffic and campaign impact

- SARIMAX performs best when campaign data is available

- Prophet handles seasonal patterns effectively

- Mobile traffic dominates page views
  
## 🛠️ Tools

- Python, Pandas, NumPy, Matplotlib, Statsmodels, Facebook Prophet
