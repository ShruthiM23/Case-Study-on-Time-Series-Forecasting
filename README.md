# Case-Study-on-Time-Series-Forecasting

# Problem Statement:
An univariate time series forecasting case study for forecasting the "Number of Tractor Sold" for 1 more year in the future by taking 10 years of historic sales data.

#### Dataset source: https://www.kaggle.com/saurav9786/time-series-tutorial/data?select=TractorSales.csv

# Project Workflow:

1. Exploratory Data Analysis<br>
2. Applying different modelling techniques(Exponential Smoothing, ARMA, ARIMA, SARIMA)<br>
3. Identifying the appropriate model wrt RMSE and MAPE<br>
4. Fitting the entire dataset for the best model to forecast data for 1 year in the future.<br>


# EDA Summary

1. Data is from January 2003 to December 2014. It has 144 records and 2 variables "Month-Year" and "Number of Tractor Sold".
2. Avg. number of tractors sold are 390 with a standard deviation of 171 and the highest number of tractors sold in a month is 871.
3. No missing values found.
4. There are no outliers present in the dataset.
5. The Sales feature is slightly right skewed as the above distribution plot tails to the right side.
6. There is seasonal peak in the sale of tractors during the month of July & August all throught the years.
7. Trend is "Multiplicative" and seasonality is "Additive" in nature.


# Final ScoreCard of various models

![image](https://user-images.githubusercontent.com/85027425/132127128-943748a3-9b2f-4fac-8651-6d0d5faf2ef6.png)

#### We will bulid full model for the TES(T=mul,S=mul) and SARIMA(1,0,1),(1,0,1,12) as showed MAPE < 5% and forecast for the future 1 year(12 months).

## 1.TES(T=mul,S=mul)

![image](https://user-images.githubusercontent.com/85027425/132127187-e1706c52-244b-4064-88b1-b2e76523f474.png)

## 2. SARIMA

![image](https://user-images.githubusercontent.com/85027425/132127207-1138d247-5a18-40e2-b32e-14d94f62cdb6.png)

# Visualizing the forecast of both the above models:

![image](https://user-images.githubusercontent.com/85027425/132127236-a5ffdb1f-767e-4df9-9cc2-bc85ddd914a7.png)
