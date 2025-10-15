# Basic Concept

This indicator measures price momentum in a smoother and less noisy way than the traditional MACD. It uses special moving averages to filter out market noise.

## Indicator Components

### 1. Green Line (ImpulseMACD) - md

This is the main line that measures momentum:

- **How it works:** Calculates the distance between the average price and its upper/lower bands
- **Above zero:** Bullish momentum (the price is above its normal range)
- **Below zero:** Bearish momentum (the price is below its normal range)
- **At zero:** No defined momentum (the price is within its normal range)

### 2. Red Line (Signal Line) - sb

This is a smoothed moving average of the green line (9 periods):

- It acts as a filter to confirm trend changes
- It moves slower than the green line

### 3. Red Histogram (ImpulseHisto) - sh

These are the vertical bars that show the difference between the green line and the red line:

- **Large bars:** Large difference between current momentum and its average (strong momentum)
- **Small bars:** Little difference (weak or changing momentum)
- **Growing histogram:** Momentum is strengthening
- **Decreasing histogram:** Momentum is weakening

### 4. Gray Line at Zero

This is simply a visual reference to the zero level.

## Trading Signals

**Bullish Signal:**
- Green line crosses above red line
- Histogram goes from negative to positive

**Bearish Signal:**
- Green line crosses below red line
- Histogram goes from positive to negative

**Divergences (important):**
- Price makes higher highs, but indicator makes lower highs = possible bearish reversal
- Price makes lower lows, but indicator makes higher lows = possible bullish reversal

## Parameters

- **lengthMA (34):** Main period for calculating momentum bands
- **lengthSignal (9):** Period for smoothing the signal