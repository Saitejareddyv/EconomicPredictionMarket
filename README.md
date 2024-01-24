# Prediction Market for macro-economic variable
(Interest rate)
## Overview.
This macroeconomic analysis focuses on predicting the United Kingdom's interest rate using machine learning models such as Linear Regression and AdaBoost Regression. Additionally, time series forecasting methods including ARCH, GARCH, ARIMA, and SARIMA are applied. The dataset spans from 2007 to 2021 and encompasses key macroeconomic factors such as GDP, unemployment, weekly earnings, deposit rate, and yield. The aim is to determine the most accurate forecasting method and provide insights into the impact of interest rate changes on the economy and banking industry
## Data-Gathering.
Data was collected from sources such as FRED and the Bank of England, initially not in monthly format. We converted the data to monthly and addressed seasonality using an Excel pivot table, rendering it a suitable dataset. The target variable is the interest rate, alongside macroeconomic factors like gross domestic product, unemployment rate, yield, weekly earnings, and deposit rate.
## Data-Cleaning.
The dataset comprises 180 rows and 7 columns, incorporating various data types, including float. The date column is maintained in Datetime format using the data frame to_datetime transformation. Given the absence of null values, no null treatment is required during the data cleaning process.
## Visulization of Data.
In this comprehensive analysis, the exploratory data analysis (EDA) process was initiated to unravel patterns, anomalies, and relationships within the dataset encompassing 180 rows and 7 columns. The primary focus was on predicting the United Kingdom's interest rate, utilizing diverse methodologies such as linear regression, AdaBoost regression, and time series forecasting models including ARCH, GARCH, ARIMA, and SARIMAX.

EDA involved a correlation matrix, heatmap, and Principal Component Analysis (PCA) to discern relationships among variables. PCA revealed that Interest rate strongly correlated with PCA 1, offering insights into the underlying factors influencing interest rates.

Machine learning models, specifically linear regression and AdaBoost regression, were applied, with AdaBoost regression demonstrating superior accuracy at 97%. The Ordinary Least Square (OLS) regression method underscored the significant impact of GDP and deposit rate on interest rates.

Time series analysis using ARCH and GARCH models indicated their lack of statistical significance in predicting future interest rates. However, ARIMA modeling, after ensuring data stationarity, resulted in an optimal model order of (0,1,1), providing accurate predictions.

SARIMAX, incorporating seasonality and exogenous factors, exhibited improved accuracy and revealed a downward trend in the forecasted interest rates from 2022 to 2026.

## Summary.
The AdaBoost regression model emerged as the most suitable for predicting interest rates among the machine learning algorithms. The combination of time series methods, including ARIMA and SARIMAX, enriched the forecasting capabilities, emphasizing the importance of considering various models for robust predictions in macroeconomic analyses. The SARIMAX model, in particular, forecasted a declining trend in interest rates for the upcoming years.
