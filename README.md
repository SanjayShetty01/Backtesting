# Backtesting

The main objective of the project is to familarise myself with coding a backtest using a custom stradegy in [Bank Nifty Index](https://www.niftyindices.com/indices/equity/sectoral-indices/nifty-bank) 


The Custom Stradegy used:

1) The all the trades are between 9:30 am to 3:15 am i.e, trade starts at 9:30 am - 9:45 am candle and all the open position till at 3:15 pm will be squared off on the same day (at 3:15 pm)

2) The buy signal (long) is sent when the 15 minute candle closes above the [VWAP](https://www.investopedia.com/terms/v/vwap.asp). And the sell signal (shorting) will be sent when the same 15 minute candle is below the VWAP trendline.  

3) Another buy signal would be sent at one tick (0.05 pts) above previous high, if the 2nd 15 minute candle after the previous one closes above the VWAP, and a stoploss of would be on 1 tick (0.05 pts) below the previous candle. 

4) If no stoploss is hit the trades would be squared off at 3:15 am. 


*Please do note that this is a random stradegy I assumed with an intention of improving my coding skills rather than improving my trading skills*


### The VWAP line over a Bank NIFTY on day one of the dataset 

![image](https://github.com/SanjayShetty01/Backtesting/blob/main/plots/plot1.png)
