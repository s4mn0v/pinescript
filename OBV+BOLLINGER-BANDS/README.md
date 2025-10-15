# Basic Concept

This indicator analyzes trading volume to confirm the strength of price trends. It combines OBV (On Balance Volume) with Bollinger Bands and a fast EMA.

## Indicator Components

### 1. OBV (On Balance Volume) - Blue Line

This is a cumulative volume indicator that measures buying and selling pressure:

- **Rises:** When the price closes higher than the previous close (buying volume)
- **Falls:** When the price closes lower than the previous close (selling volume)

**Key concept:** If the OBV rises while the price rises, it confirms that the uptrend is strong (there is real volume behind the movement).

### 2. Bollinger Bands applied to OBV

Instead of being applied to the price, these bands are applied to the OBV to measure its volatility:

- **Middle Band (yellow dotted):** 20-period SMA of OBV
- **Upper Band (red dotted):** Indicates high buying pressure
- **Lower Band (green dotted):** Indicates high selling pressure
- **Light green fill:** Area between the bands

### 3. OBV 10 EMA (purple line)

This is a fast average of the OBV that detects changes in momentum more quickly.

### 4. Color Fill between 10 EMA and Middle Band

- **Green:** 10 EMA above the middle band = upward momentum in volume
- **Red:** EMA 10 below the middle band = bearish momentum in volume

## How to Interpret It

**Divergences (most important):**
- **Bullish divergence:** Price makes lower lows, but OBV makes higher lows (possible upward reversal)
- **Bearish divergence:** Price makes higher highs, but OBV makes lower highs (possible downward reversal)

**Trend confirmation:**
- Strong uptrend: Price rises AND OBV rises (green fill)
- Strong downtrend: Price falls AND OBV falls (red fill)

**Momentum signals:**
- EMA 10 crosses above the middle band = increase in buying pressure
- EMA 10 crosses below the middle band = increase in selling pressure