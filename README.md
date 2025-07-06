# Problem Statement


In this problem statement we have to develop algorithmic trading strategies for the BTC/USDT
cryptocurrency market, aiming to outperform benchmark returns.
We have to develop a trading strategy for the BTC-USDT market that maintains narrow
drawdowns with a good time to recovery rate and beats benchmarks 50-70% of the time.

# Strategy Overview

For our strategy , we have used a combination of various indicators like Ichimoku Cloud ,
MACD , RSI , Bollinger Bands , OBV , Volume Indicator , ATR .
We have also used Regime Switching technique , which helps us to change the span or
window period of various indicators based on the current volatility.
We have selected indicators that help in identification of the trend and its strength.
To denoise the data we have used Heikin Ashi Candles .
For our strategy , we have used the following Risk Management Methods ->
Normal take profit , Trailing take profit , ATR stop loss , Max drawdown limit to close
trades on next day , Intraday price change limit , Daily close change limit .

# Development Process

Analyzing Data


1) We began first by analyzing the stock data provided . The data was of the period
2020-2023. We were provided with data of different intervals from minute wise data
to daily data .
The close price plot of the daily data showed that the BTC-USDT market was very
volatile during this period . The market first rose and achieved its peak then it began
falling ,but rose again and achieved a new global peak and then again started falling.


2) Analyzing the data we interpreted that volume change plays a very important role in
identifying strong trends as trend reversals are accompanied by drastic changes in
volume .
Therefore we developed an indicator which detects a drastic change in volume by
taking the difference of ratio of a fast exponential moving average to a slow
exponential moving average . This indicator helped us to identify the various points
of drastic change in volume which can be the potential points of trend reversal or
beginning of a strong trend . Now to identify the trend , we combined this Volume
Indicator with OBV and Ichimoku Cloud Indicator to generate long and short signals


3) Then we used combinations of other technical indicators like MACD , RSI , Bollinger
Bands , ATR , Ichimoku Cloud and On Balance Volume.
    i) MACD and Ichimoku Cloud - To identify trends , bullish or bearish.
   ii) RSI and Bollinger Bands - To measure strength of trend and identify overbought
       or oversold conditions.
  iii) ATR - To measure the current volatility.
   iv) OBV - To measure positive and negative volume flow and analyze the trading
       direction.


4) Our final strategy is a combination of these different indicators . We have chosen
indicators that help identify points of entry into long and short trades on the basis
of trend direction , strength and momentum of trend as well as volume changes.


5) The final step of the development process was Strategy Optimization .


 i) We optimized the various indicators to suit the BTC-USDT market by tweaking the
 various parameters of these indicators .


 ii) We developed new and better risk management methods like Intraday price
 change limit , Daily price change limit , trailing stop loss and take profit to protect
 the capital and make the strategy more robust and profitable.

