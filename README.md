# Time-Series-Models: Forecasting Net Prophet


## Step 1: Find Unusual Patterns in Hourly Google Search Traffic


### ***Question:*** 
Did the Google search traffic increase during the month that MercadoLibre released its financial results?

### ***Answer:*** 
* Traffic did increase from ~35,173 to ~38,181 which is ~8.6% traffic increase in May 2020 vs. the historical norm. We'd need to run a statistical significance test to know whether this is a significant traffic increase.


## Step 2: Mine the Search Traffic Data for Seasonality

### ***Question:***
Does any day-of-week effect that you observe concentrate in just a few hours of that day?

### ***Answer:*** 
* Yes across all days, there seems to be a concetration in the late night, early morning hours of the day from ~2:00 - 03:00 hours

### ***Question:*** 
Does the search traffic tend to increase during the winter holiday period (weeks 40 through 52)?

### ***Answer:*** 
* Yes there seems to be an increase from week 41 through week 51. This looks like a Christmas shopping season ramp-up before the post-Christmas crash. Having said this, the ramp-up during this period starts from near the yearly low point and the peak is still lower than earlier in the year (week 4 peak).


## Step 3: Relate the Search Traffic to Stock Price Patterns

### ***Question:*** 
Do both time series indicate a common trend that’s consistent with this narrative?

### ***Answer:*** 
* No, trend is not consistent with the narrative

### ***Question:*** 
Does a predictable relationship exist between the lagged search traffic and the stock volatility or between the lagged search traffic and the stock price returns?

### ***Answer:*** 
* No, a predictable relationship does not exist, the correlation coefficients are way too low to indication any sort of relationship between Lagged Search Returns and Stock returns or stock volatility.


 ## Step 4: Create a Time Series Model with Prophet

### ***Question:*** 
How's the near-term forecast for the popularity of MercadoLibre?

### ***Answer:*** 
* Near-term forecasts seem to follow seasonal patterns and are declining heading into November and then show the traditional ramp-up into Christmas. The near-term dip seems to be greater than previous years.

### ***Question:*** 
What time of day exhibits the greatest popularity?

### ***Answer:*** 
* Midnight seems to exhibit the greatest popularity

### ***Question:*** 
Which day of week gets the most search traffic?

### ***Answer:*** 
* Tuesday gets the most search traffic

### ***Question:*** 
What's the lowest point for search traffic in the calendar year?

### ***Answer:*** 
* October seems to be the lowest time of the year for search traffic


 ## Step 5 (Optional): Forecast Revenue by Using Time Series Models

### ***Question:*** 
For example, what are the peak revenue days? (Mondays? Fridays? Something else?)

### ***Answer:*** 
* Peak revenue days are Wednesday

### ***Answer:***  
* The quarter sales forecast for 7-1-2020 to 9-30-2020 is as follows:
Best Case: $2,338.75
Expected Case: $2,163.70
Worst Case: $1,987.96
