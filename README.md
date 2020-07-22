# Time Series Analysis with Bitcoin

<img src="images/Bitcoin%20pic.jpeg" width="650">

## Introduction:
I am building time series models to see how well they can predict Bitcoin prices.

## Objective:
To show an investment advisor or client whether an ARMA, ARIMA or FB Prophet model is useful to predict Bitcoin prices.

## The Dataset:
The dataset consisted of daily Bitcoin prices from 2015 to 2019, sourced with an API call from YahooFinance. In my first round of modeling, 2015-2018 were used as training set while 2019 was used as the validation set. In my second round of testing, the whole 5 years were used as the training set(2015-2019) and January 2020 was used as the validation set.

<img src="images/Graph%20of%20prices%2C%20rolling%20mean%20and%20rolling%20std.png" width="650">

## Skills Required to Complete:
The skills used to complete this project consisted of sourcing data by API, preprocessing data, EDA, transforming data to obtain stationarity, running the Autocorrelation Function and Partial Autocorrelation Function and selecting a model based on RMSE scores and using Python to make visualizations with Pandas.

## What I Posted on Github:
There are 2 notebooks posted on Github. The first notebook, 'Mod_4 Project.ipynb', is the main working notebook. The second, 'Experimenting with different transformations.ipynb', is only a working notebook where I was experimenting with different transformations.

## Questions I Posed:
1. Which model performed best and why?
2. What are the shortcomings of the model?

## Modeling Results (RMSE):

First round:
 1. ARMA 4,762
 2. ARIMA 2,953
 3. FB Prophet 5,145
 
Second round:
 1. ARIMA 1,319
 <img src="images/2nd%20round%20-%20ARIMA.png" width="650">
 
 2. FB Prophet 1,642
 <img src="images/2nd%20round%20-%20FB%20Prophet.png" width="650">

## Recommendations:
The ARIMA model performed the best in both rounds. However, I would not recommend using this model because it is a linear model. Also, the Bitcoin prices were a 'random walk' and therefore an ARIMA model would be useless.

## Future Steps:
1. Try to improve the ARIMA model by combining it with a sentiment analysis model to add exogenous variables.
2. Build a long short-term memory neural network to try and make better predictions.

## Presentation Link:
https://docs.google.com/presentation/d/1ZgO0r6g-MSQGYJCV7vbbpmy7CSdD6A2ibN52b9_22-c/edit?usp=sharing

## References for Images in Presentation (in order):
https://analyticsindiamag.com/all-you-need-to-know-about-the-2018-cryptocurrency-slump/ \
https://www.danielstrading.com/2017/12/12/bitcoin-commodity-currency \
https://www.finextra.com/the-long-read/40/bitcoin-halving-what-does-this-mean-and-what-will-its-effect-be
