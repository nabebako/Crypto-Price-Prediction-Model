# Cryptocurrency Price Prediction Model Overview
This is a school project for year 11 computer class:
Choose one or several of your favorite cryptocurrencies.  Develop a couple of mathematical models in python which attempt to predict the future and guess the prices of these cryptocurrency.  After your models have been developed, run your program every day for up to one week.  Collect data in regards to how close each model was to correctly predicting the cryptocurrency price.  Write a report discussing the pros and cons of your models.  Discuss which model performed the best. 
> Now, I don't really know how to write a readme.md, so this is what we got.

-------

# Cryptoprice modelling Objective

Find data, it might be more interesting to find data for less popular coins.  A lot of sophisticated models will already exist for Bitcoin/ Ethereum.   It would be more exciting to model coins like ravencoin or presearch.  It is important to collect enough data.  It will probably be best to find/collect several months worth of data and then do weekly forecasting.

Choose 3-4 mathematical prediction models and a control:

- Control - The control will simply predict that the future cryptocurrency price on a given day will be the same as the price 7 days (1 week) prior.  

- Polynomial Regression - you can use your data to build a linear or polynomial regression line.  Use this line to predict future values.

- KNN Regression - We learned how to implement the knn algorithm in class, you can actually use this algorithm to predict the future.

- Facebook's Prophet (local Bayesian structural time series model) - This is a python package that you can install.  

- ARIMA - Auto Regressive Integrated Moving Average.  An example.

- ADABOOST Regression - I have heard of state of the art forecasting using this method.  I'm not sure how complicated this will be to implement.


Start implementing each model in python.

Use models to generate 1-2 weeks of predictions.

After 1-2 weeks have passed, analyze how well each model did at predicting the value.

Create a Google Slides presentation.  Your presentation should include:

1. Overview of the project, why it is interesting, how it can be useful in the real world.
2. Explanation of how each model you used in the project works.
3. Explanation of the data, what data points are in your data set?  How was the data collected?
4. Analysis of data: show graphs and calculations.
5. Conclusions:  which model performs the best.  How could you improve your project? What lessons did you learn?


---
# Analysis Results

Mean Absolute Percentage Error Chart using 70:30 train-test ratio

| Coin                  | ADA                   | ETH                   | DOGE                  | SOL                   |
| --------------------- | --------------------- | --------------------- | --------------------- | --------------------- |
| ARIMA                 | 3.46 %                | 4.0 %                 | 3.62 %                | 3.46 %                |
| Polynomial Regression | -                     | 6.82 %                | -                     | -                     |
| KNN Regression        | 1.36 %                | 1.83 %                | 1.44 %                | 1.93 %                |
| Adaboost Regression   | -                     | -                     | -                     | -                     |


Data gathered from <a href = "https://www.coindesk.com/">CoinDesk</a>
