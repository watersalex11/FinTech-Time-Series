#Unit 10 HW 
## A Yen for the Future
### Alex Waters 7/12/20
---
**Time-Series Forecasting**

![alt text](settle.PNG)
Question:  Based on the plot above, we can see a long-term strengthening of the Japanese Yen against the Dollar. There do seem to be some more medium, 1-3 year consistent trends, but on a daily basis, there are a lot of short-term ups and downs.

Answer:  Overall trajectory over the span of the dat is generally an up trend with some significant peaks and then drops.
---
*Hodrick-Prescott Filter*
![settle vs trend](settle_v_trend.PNG)
The settle and trend price are very closely matched.
![hp noise](noise.PNG)

---
*ARMA*

![arma results](arma_results.PNG)
Notice that the p value is not less than .05.
![5 day returns forcast arma](5_day_arma.PNG)
---
*ARIMA*
![arima results](arima.PNG)
Notice p value is greater than .05.
![5 day arima](5_day_arima.PNG)
The value of the yen appears to be rising over the next 5 days.
---
*GARCH*
![GARCH results](garch_results.PNG)
The p value for omega and alpha[1] are much less than .05.

![GARCH Forecast](garch_forecast.PNG)
Based on the upward trend of the forecast the volatility looks to increase.
---

**Linear Regression Forecasting**
![predicted vs actual](linear_regression.PNG)

rmse for in-sample:  0.5665389565201941 
rmse for out-of-sample: 0.4152118225942089
The out of sample rmse is less than .5 as is a better model, but a lower rmse would have been preferable.