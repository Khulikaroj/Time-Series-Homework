# Time-Series-Homework

## Time-Series Forecasting 

### ARMA Model Evaluation

All estimated parameters in ARMA (2,1) model are statistically significant at more than 95% confidence level. Projected return in the next 5 days shows upward trends in Yen Futures. Acccroding to this result, the model suggest us to buy Yen Futures for the next 5-day investment horizon.

### ARIMA Model Evaluation

ARIMA(5,1,1) Model also suggest the same as ARMA(2,1) model, buy Yen. However, none of estimated parameters from ARIMA(5,1,1) model are statistically significant at 95% confidence level.

This problem might arise from model specification. Estimated parameter would be statistically significant if we use ARIMA(1,1,1) as ACF and PACF suggest. ARIMA(1,1,1) also give lower AIC and BIC which mean better model specification compared to ARIMA(5,1,1). 

From ARIMA(1,1,1), the forcasted Yen price increase in the next 5 days and suggest we should buy Yen Futures and hold position for the next 5 days. 

### GARCH Model Evaluation

With GARCH(p=2,q=1) model, one estimated parameter is not statistically significant so I run another GARCH model with p=1, q=1 to compare the result. This turn out that all estimated parameters are statistically significant at 95% confident interval and AIC,BIC are slightly improved. Both models suggest that volatility of Yen Futures price will increase in the next 5 days. However, R-square of both models are very low and suggest that these models scarcely fit to real data. Hence, using the prediction should be done with caution that there might be room for error.

### Conclusions

Based on ARMA and ARIMA trend analysis, I would buy Yen Futures and hold the position at least 5 days. However, prediction from the model should be reestimated along the investment horizon and be aware of structural break. 

Given GARCH analysis, volatility of Yen Futures price is expected to increase in the 5-day horizon. However, fitness of the model is very low and there might be large room for error from estimation.

Based on the model evaluation, I would feel more confident to trade Yen Futures position based on estimated price. However, I would feel less conficdent in using predicted risk to trade Yen derivatives  given low fitness of the model. Trading derivatives is more risky and need more accuracy of model prediction. With low accuracy or precision, I might end up being charged with large margin call if there is anything beyond the model forecast.

## Regression Analysis

Linear regression model of return on 1-day lagged return perform better on out-of-sample data compared to in-sample data.
