# Vector Auto Regression (VAR) and VARMAX Model for Time Series Forecasting

## Introduction

This project explores the use of Vector Auto Regression (VAR) and VARMAX models for time series forecasting using macroeconomic data. VAR models are powerful tools in econometrics for analyzing and forecasting multivariate time series data.

## Dataset

The dataset used in this project contains macroeconomic variables including real gross national product (rgnp) and unit labor cost (ulc). The data can be accessed [here](https://raw.githubusercontent.com/selva86/datasets/master/Raotbl6.csv).

## Exploratory Data Analysis

### Visualizing Time Series

The initial step involves visualizing the time series data to understand trends and patterns. Each series is plotted individually to observe their behavior over time.

### Stationarity Check

Before modeling, stationarity of the time series is checked using the Dickey-Fuller test. If a series is non-stationary, differencing is applied until stationarity is achieved.

### Granger Causality Test

The Granger causality test is conducted to determine if there is a causal relationship between ulc and rgnp. This helps in understanding if past values of ulc can predict rgnp and vice versa.

## Model Building

### VAR Model Selection

The order (lags) for the VAR model is selected based on minimizing the Akaike Information Criterion (AIC). This step helps in choosing the optimal lag order for the model.

### VARMAX Model

The VARMAX model is utilized for forecasting. Here, the VAR model is extended to accommodate external variables or exogenous factors. In this case, no exogenous variables are included, so only the autoregressive (AR) terms are specified.

### Model Evaluation

The fitted VARMAX model is used to make forecasts for the test period. Evaluation metrics such as Root Mean Squared Error (RMSE) are calculated to assess the accuracy of the forecasts compared to the actual test data.

## Conclusion

This README provides an overview of applying VAR and VARMAX models to macroeconomic time series forecasting. These models are useful for capturing relationships between multiple variables and making accurate predictions based on historical data.
