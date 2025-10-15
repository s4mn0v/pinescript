# Basic Concept

This strategy automatically buys and sells based on the crossover of two lines: a fast EMA (9 periods) and a slow EMA (21 periods).

## What is an EMA?

EMA = Exponential Moving Average. It is a line that smooths the price and shows the average trend. The fast EMA (9) reacts faster to price changes than the slow EMA (21).

## Buy and Sell Signals

**BUY:** When the 9 EMA crosses above the 21 EMA
- It means that the price is rising strongly
- The strategy enters a long position (buy)

**SELL:** When the 9 EMA crosses below the 21 EMA
- This means that the price is falling or losing momentum
- The strategy closes the position (sells)

## Strategy Parameters

- Initial capital: 1000 USDT
- Use 100% of capital in each trade
- Only allow 1 open trade at a time (pyramiding = 1)
- You can set the start and end dates for the backtest
- Option to color the background: green when EMA 9 > EMA 21, red when EMA 9 < EMA 21

## Visualization

- Green “Buy” label appears below the candle when there is a buy signal
- Red “Sell” label appears above the candle when there is a sell signal

Translated with DeepL.com (free version)