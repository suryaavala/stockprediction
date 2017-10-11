# Stock Market Price Prediction

# Review

# Data

The main component in any **Market prediction** problem is the **price**. But this time we also need another 3 features. We are going to use **three popular technical indicators** that (hopefully) will help the model predict the price (as they help human traders to do the same task).

## Technical Indicators

There are A LOT of different technical indicators for market analysis. The universe of "technical analysis" for trading is vast. Most of it is out of our scope, so we're just going to present three simple technical indicators, each specialized in a different task.

### Trend indicator
<a href="http://www.investopedia.com/university/technical/techanalysis3.asp">What is Trend?</a>
#### MACD
The Moving Average Convergence/Divergence oscillator (MACD) is one of the simplest and most effective momentum indicators available. The MACD turns two trend-following indicators, moving averages, into a momentum oscillator by subtracting the longer moving average from the shorter moving average.
<img src="http://i68.tinypic.com/289ie1l.png">


### Momentum indicator
<a href="http://http://www.investopedia.com/terms/m/marketmomentum.asp">What is Momentum?</a>
#### Stochastics Oscillator
The Stochastic Oscillator is a momentum indicator that shows the location of the close relative to the high-low range over a set number of periods.
<img src="http://i66.tinypic.com/2vam3uo.png">


### Volume indicator
<a href="http://www.investopedia.com/terms/v/volume.asp">What is Volume?</a>
#### Average True Range
Is an indicator to measure the volalitility (NOT price direction). The largest of:
- Method A: Current High less the current Low
- Method B: Current High less the previous Close (absolute value)
- Method C: Current Low less the previous Close (absolute value)

<img src="http://d.stockcharts.com/school/data/media/chart_school/technical_indicators_and_overlays/average_true_range_atr/atr-1-trexam.png" width="400px">

Calculation:<br>
<img src="http://i68.tinypic.com/e0kggi.png">

# Models

Two Neural Networks based models are presented. Both of them are implemented with Tensorflow.

## Deep Regressor

Just a regression model with a Deep Neural Network architecture. Details in the corresponding Notebook "Currency_Market_Predictor_DeepRegressor.ipynb"

## Recurrent Neural Network

A (more appropiate) recurrent neural network model. Details in the corresponding Notebook "Currency_Market_Predictor_RNN.ipynb"

# Results

### EUR-USD
A pair of plots is worth many thousand words.

-Price vs Prediction w/ Deep Regressor
<img src="https://github.com/alberduris/SirajsCodingChallenges/blob/master/Stock%20Market%20Prediction/src/PriceVsPred_DeepRegressor.PNG?raw=true">

-Price vs Prediction w/ Recurrent Neural Network
<img src="https://github.com/alberduris/SirajsCodingChallenges/blob/master/Stock%20Market%20Prediction/src/PriceVsPred_RNN.PNG?raw=true">

### Bitcoin
Price vs Prediction w/ RNN
<img src="https://github.com/alberduris/SirajsCodingChallenges/blob/master/Stock%20Market%20Prediction/src/PriceVsPredict_BTCUSD_RNN.PNG?raw=true">

### Ethereum
Price vs Prediction w/ RNN
<img src="https://pbs.twimg.com/media/DJ3uIWbU8AABS6C.jpg:large">

## Dependencies for challenge


* numpy
* tensorflow

## Dependencies for Full Notebook

* matplotlib (for plotting)
* pandas (for dataset manipulation)

### References


<a href="http://www.investopedia.com/university/technical/techanalysis3.asp">Technical Analysis - The use of Trend - Investopedia</a><br>
<a href="http://http://www.investopedia.com/terms/m/marketmomentum.asp">Momentum Market - Investopedia</a><br>
<a href="http://www.investopedia.com/terms/v/volume.asp">Volume - Investopedia</a><br>
<a href="https://www.youtube.com/watch?v=LhtnECml-KI">Siraj Raval - Youtube - Quantum Computing - The Math of Intelligence #10</a><br>
<a href="https://github.com/alberduris/SirajsCodingChallenges">alberduris/SirajsCodingChallenges</a>
