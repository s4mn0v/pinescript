# Basic Concept

This indicator combines two technical analysis tools: EMAs to identify trends and Bollinger Bands to measure volatility and overbought/oversold levels.

## Indicator Components

### 1. Bollinger Bands

These are three lines that form a channel around the price:

- **Upper Band (red):** Indicates a possible overbought zone
- **Middle Band (blue dotted):** This is the 20-period moving average, showing the average price
- **Lower Band (green):** Indicates a possible oversold zone
- **Purple Fill:** The area between the upper and lower bands shows market volatility

**Configuration:**
- Uses a 20-period SMA by default
- Standard deviation of 2.0
- You can change the type of moving average (SMA, EMA, WMA, etc.)

### 2. EMAs (Exponential Moving Averages)

- **EMA 9 (red line):** Fast average that closely follows the current price
- **EMA 21 (green line):** Slower average that indicates the medium-term trend

### 3. Color Fill between EMA 9 and Middle Band

- **Green:** When EMA 9 is above the middle band (uptrend)
- **Red:** When EMA 9 is below the middle band (downtrend)

## How to Interpret It

**Bullish Signals:**
- Price above the middle band
- EMA 9 above the middle band (green fill)
- EMA 9 above EMA 21

**Bearish Signals:**
- Price below the middle band
- EMA 9 below the middle band (red fill)
- EMA 9 below EMA 21

**Volatility:**
- Wide bands = high volatility
- Narrow bands = low volatility (possible breakout coming)

Translated with DeepL.com (free version)