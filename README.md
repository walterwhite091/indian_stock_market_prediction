# indian_stock_market_prediction
Summer Project ( 2018 )


We have set our prior objective as the analysis of the present scenario of the Indian Stock Market so as to understand and try to create a better future scope for investment. We have collected data on the monthly closing stock indices of BSE for ten years and based on these we have tried to develop an appropriate model  which would help us to forecast the future unobserved values of the Indian stock market indices.We have established ARIMA model as the best fitted 
model to describe the observed time series and forecast future value.
ARIMA is  "Auto Regressive Integrated Moving Average". This model is classified as an "ARIMA(p,d,q)" model where
p is the number of autoregressive terms.
d is the number of non-seasonal difference needed for stationarity .
q is the number of lagged forecast errors in the pridiction equation.

What we do -

1 - Firstly we check for stationarity of our data.
 "Stationarity" implies that the series remains at a fairly constant level over time. If a trend exists then the time series is called as non-stationary . We found that our data as non-stationary.

2 - Differencing - We take the value in the current period and subtract it by the value from the previous period. We have to do this several times to make the data stationary. This is the Integrated component which is d in the model terms.
In my case , data become stationary after 1st differencing .
So, d =1 in ARIMA parametre . 

3-We have decided the  p , q terms by Autocorrelation PLOT and Partial autocorrelation PLOT . 
We need to check the value where the graph cuts off or drop to Zero for the first time ,
In our case we get 
p=1 (From Partial autocorrelation PLOT  )
q=1 (From Autocorrelation PLOT )

4-Now after finding all the parameter of ARIMA (p=1,d=1,q=1), We have applied the ARIMA model by passing these parameter .

Result:
We got pridiction for our future value and 95% confidence interval.
