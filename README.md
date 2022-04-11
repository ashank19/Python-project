# Python-project
Ethereum crypto prediction
The current trend in the era of investment is trading in the cryptocurrency market. 
In the last couple of years, the cryptocurrency market went from being speculation to amassing enormous volumes of  traffic
of  currency  being  traded  every  day.  Even  after  being  such  a  popular  method  of investment,  
there  is  still  a  lack  of  prediction  methods  for  the  extremely  sensitive  and  volatile cryptocurrency market.

Introduction
Using this  project,  we  plan to  incorporate  the  parameter  of  predictionfor  the  price  of  popular cryptocurrency “Ethereum” usually abbreviated
as ETH in the markets. For this, an extremely vast dataset is being utilized which contains information about multiple cryptocurrencies. 
Time Series Forecasting methods will be used for the predictions.

Problem Statement
•	Analyze the data corresponding to Ethereum and find out trends or interesting patterns
•	Predict the closing price of ETH using Time Series Forecasting
•	The database schema consists of two tables: Dailylisting and Asset 
Details![image](https://user-images.githubusercontent.com/41359809/162677950-f0716744-0e39-474b-88d8-9ee85480b2a9.png)

Data Information
The dataset downloaded from Kaggle contains information on historic trades for several crypto assets, such as Bitcoin and Ethereum. The dataset training file consists of 10 columns. The description of the columns is as below: 
•	timestamp - A timestamp for the minute covered by the row. 
•	Asset_ID - An ID code for the crypto asset. For eg. asset_id == 6 for ETH
•	Count - The number of trades that took place this minute. 
•	Open - The USD price at the beginning of the minute. 
•	High - The highest USD price during the minute. 
•	Low - The lowest USD price during the minute. 
•	Close - The USD price at the end of the minute. 
•	Volume - The number of crypto asset units traded during the minute. 
•	VWAP - The volume-weighted average price for the minute. 
•	Target - 15 minute residualized returns 
![image](https://user-images.githubusercontent.com/41359809/162677993-ff2eb08c-18be-40c5-a9aa-82666a53e2b8.png)

Database Operations
we have created a database called ‘crypto’ and dumped our dataset into table ‘Dailylisting’, then fetched two columns from table ‘timestamp’ 
as one of the features for prediction and ‘Close’ a target variable. Then performed predictions using time series algorithms on the fetched data.

Conclusion
We compared the metrics of the two models and found that exponential smoothing has much lower RMSE, MAE as compared to the auto_arima model. The exponential smoothing model predicted the prices which were quite following actual prices. 
We have also used Streamlite which is an open-source framework to build web apps to visualize time-series decomposing which helped us to verify the various trends and volatility of Ethereum. We have currently performed a univariate analysis. In the future, we can explore multivariate analysis and can explore more algorithms that can give us better results in terms of future price predictions
![image](https://user-images.githubusercontent.com/41359809/162678359-faf03b1f-871d-40ee-843d-c6c648ac67a2.png)


References / Useful Links:
•	Dataset Link: https://www.kaggle.com/c/g-research-crypto-forecasting/data 
•	What is Cryptocurrency? https://en.wikipedia.org/wiki/Cryptocurrency  
•	What is Time Series Forecasting? https://en.wikipedia.org/wiki/Time_series 
•	Exponential Smoothing: https://en.wikipedia.org/wiki/Exponential_smoothing 
•	UBBox link to code: https://buffalo.app.box.com/folder/150455294788 
![image](https://user-images.githubusercontent.com/41359809/162678384-f4b85cd0-8ada-46df-8c92-539aff374c87.png)






