# Unit 10—A Yen for the Future

![Yen Photo](Images/unit-10-readme-photo.png)

## Background

The financial departments of large companies often have to make foreign currency transactions when doing international business, while hedge funds are also interested in anything that will provide an edge in predicting currency movements. Hence, both are always eager to gain a better understanding of the future direction and risk of various currencies. 

In this assignment, many time series have been used in order to predict future movements in the value of the Canadian dollar versus the Japanese yen.

The following tasks are done:

1. Time series forecasting
2. Linear regression modelling

- - -

### Files

[Time-Series Starter Notebook](Starter_Code/time_series_analysis.ipynb)

[Linear Regression Starter Notebook](Starter_Code/regression_analysis.ipynb)

[CAD/JPY Data CSV File](Starter_Code/cad_jpy.csv)

- - -

#### Time-Series Forecasting

In this notebook, historical CAD-JPY exchange rate data has been loaded and applied time series analysis and modelling to determine if there is any predictable behaviour.

The steps are outlined in the time series starter notebook to complete the following:

1. Plotting the Settle price to check for long or short-term patterns.

2. Decomposition using a Hodrick-Prescott filter (decompose the settle price into trend and noise).

3. Forecasting returns using an ARMA model.

4. Forecasting the exchange rate price using an ARIMA model.

5. Forecasting volatility with GARCH.

Using the results of the completed time series analysis and modelling the following questions were answered:

1. Based on your time series analysis, would you buy the yen now?
2. Is the risk of the yen expected to increase or decrease?
3. Based on the model evaluation, would you feel confident in using these models for trading?

#### Linear Regression Forecasting

In this notebook, a Scikit-Learn linear regression model was built to predict CAD/JPY returns with *lagged* CAD/JPY futures returns and categorical calendar seasonal effects (e.g., day-of-week or week-of-year seasonal effects).

In the regression_analysis starter notebook, the following was completed:

1. Data preparation (creating returns and lagged returns, and splitting the data into training and testing data)
2. Fitting a linear regression model.
3. Making predictions using the testing data.
4. Out-of-sample performance.
5. In-sample performance.

Using the results of the linear regression analysis and modelling the following question was answered:

* Does this model perform better or worse on out-of-sample data compared to in-sample data?

- - -