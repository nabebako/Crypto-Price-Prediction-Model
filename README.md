# Cryptocurrency Price Prediction Model Overview
This is a high school project for year 11 computer class:
choose one or several of your favorite cryptocurrencies.  Develop a couple of mathematical models in python which attempt to predict the future prices of these cryptocurrencies.  After your models have been developed, run your program every day for up to one week.  Collect data in regards to how close each model was to correctly predicting the cryptocurrency price.  Write a report discussing the pros and cons of your models.  Discuss which model performed the best.

# Cryptoprice Modelling Objective

We will try to assert the accuracy of various models when doing analysis on crypto prices. We had gathered four datasets from <a href = "https://www.coindesk.com">CoinDesk</a>: ADA, ETH, DOGE, and SOL, each having differnt trends and volitility. We will conduct weekly forecasting analysis on said datasets using 6 approches listed below:

- Control - predicts based on prices from a specific window of time prior.

- Polynomial regression - a linear or polynomial regression line use predict future values.

- KNN (k-nearest neighbors) regression - uses similar traits of a given day to determine prices.

- Facebook's Prophet (local Bayesian structural time series model).

- ARIMA (Autoregressive integrated moving average) - consider correlation of lags (passed values) to predicts values.

- AdaBoost (Adaptive boost) regression - a collection of weak learners that cover each other weaknesses.


Implementation will be done using python in Jupyter Notebook in combination with third party libraries: pandas, NumPy, Matplotlib, scikit-learn, statsmodels, and prophet.
We will measure accuracy using two methods. One measures the mean absolute precentage error (MAPE) on a 70:30 train-test-split ratio datasets with rolling forecasting - refitting modes every time a new day is predicted with that day's values. The other measures the accuracy accross the span of 2 weeks and compare each model with one another also using MAPE as the metric.

# Analysis Results

MAPE Chart using 70:30 train-test ratio

| Coin                  | ADA                   | ETH                   | DOGE                  | SOL                   |
|-----------------------|-----------------------|-----------------------|-----------------------|-----------------------|
| ARIMA                 | 3.46%                 | 4.0%                  | 3.62%                 | 3.46%                 |
| Polynomial Regression | 3.89%                 | 4.87%                 | 4.47%                 | 4.68%                 |
| KNN Regression        | 1.36%                 | 1.83%                 | 1.44%                 | 1.93%                 |
| Adaboost Regression   | ~ 3.95%               | ~ 5.58%               | ~ 7.64%               | ~ 4.55%               |
| Facebook Prophet      | -                     | -                     | -                     | -                     |
| Control (baseline)    | 4.94%                 | 6.38%                 | 8.93%                 | 6.80%                 |

Data gathered from <a href = "https://www.coindesk.com/">CoinDesk</a>