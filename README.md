# Time Series Forecasting for Tax Revenue

# Overview
This project explores time series forecasting techniques to predict quarterly state and local government tax revenue in the U.S. from 2009 to 2023. The dataset is sourced from the U.S. Census Bureau, and various regression and time series models were applied to analyze trends and predict future values.

# Technologies Used
R (forecast, zoo, ggplot2, tseries libraries)

Time Series Analysis (ARIMA, Auto-ARIMA, Quadratic Trend, Exponential Model)

Model Evaluation Metrics (RMSE, MAPE)

# Methodology
## Data Preprocessing
Removed incomplete records (1992-2008)

Used quarterly data from 2009-2023

Partitioned dataset into training (2009-2019) and validation (2020-2023)

## Exploratory Data Analysis (EDA)
Identified trends and seasonality

Used autocorrelation (ACF) and differencing for stationarity assessment

## Models Implemented
Quadratic Trend Model

Quadratic Trend + Seasonality

Exponential Model

ARIMA (1,1,1)(1,1,1)

Auto-ARIMA

# Results & Model Performance
Model	RMSE (Validation)	MAPE (Validation)

ARIMA Model with Seasonality	6504.35	2.30%

Auto-ARIMA	6316.58	2.41%

Quadratic Regression Model	15376.13	2.58%

Quadratic Model with Seasonality	15201.87	2.69%

Exponential Model	18680.78	3.05%

Naive Forecast	20251.23	2.61%

Seasonal Naive Forecast	29619.99	5.48%

# Key Findings
ARIMA Model with Seasonality provided the most accurate forecast with the lowest RMSE and MAPE.

Quadratic models captured long-term trends but lacked adaptability to fluctuations.

Exponential models underperformed due to high variance.

Auto-ARIMA performed well but did not significantly outperform manually tuned ARIMA.

# Future Enhancements
Incorporate external factors (e.g., economic indicators, policy changes)

Test deep learning models like LSTM for time series forecasting

Deploy an interactive dashboard for real-time trend analysis

# Contributors
Garima Vijay
