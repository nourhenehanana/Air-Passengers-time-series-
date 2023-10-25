# Air-Passengers-time-series-
Given  a dataset that contains monthly totals of international airline passengers, we will perform time series analysis and forecasting  to reveal whether there is a consistent increase or decrease in the number of passengers over the months or years and to make predictions about future values based on historical data.

# Steps
1- Perform exploaratory data analysis 
2- Decomposition of the data
3- Check stationarity using dicky fuller test : The Dickey-Fuller test (DF test) is a statistical test used to determine whether a time series data set is stationary or non-stationary. In a stationary time series, the statistical properties (such as mean, variance, and covariance) remain constant over time, whereas in a non-stationary time series, these properties change over time.

The DF test is based on a regression model that includes the lagged values of the dependent variable and a time trend. The null hypothesis of the DF test is that the time series data set has a unit root, which implies that it is non-stationary. The alternative hypothesis is that the time series data set is stationary.

If the calculated test statistic is less than the critical value, the null hypothesis is rejected, and the time series data set is considered stationary. On the other hand, if the calculated test statistic is greater than the critical value, the null hypothesis is not rejected, and the time series data set is considered non-stationary.

The Dickey-Fuller test is widely used in economics and finance to test the stationarity of financial and economic time series data, such as stock prices, exchange rates, and macroeconomic variables. 
In our case we rejected the null hypothesis as we find out the results of the dickey fuller test show that the test statistic is less than 1% of critical value that tells us that we are 99% confident that the seriesis stationary.
4- Modeling using ARIMA algorithm after der determing p and q value using respectively the pacf and ACF plots. 
![image](https://github.com/nourhenehanana/Air-Passengers-time-series-/assets/93352403/ccb86834-2e08-427a-9384-fbd17e814466)
The AFC curve crosses the upper confidence value when the lag value is between zero and 1 thus the optimal value of Q and the ARIMA model must be 0 or 1. 
![image](https://github.com/nourhenehanana/Air-Passengers-time-series-/assets/93352403/0aa5e4d9-b2a2-454c-a6cd-8d19b59318c5)
The pacf curve drops to zero between lag values 1 and 2 thus the optimal value of p in the ARIMA model is 1 or 2. 

