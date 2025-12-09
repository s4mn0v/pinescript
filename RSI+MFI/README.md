# RSI + MFI Combined

**What you achieve:** Confirm whether a signal is REAL or FALSE by comparing price (RSI) with volume (MFI).

## The 4 Situations

### 1. Both Overbought (RSI >70 + MFI >80)

**Meaning:** High price WITH a lot of money coming in **Action:** STRONG SIGNAL of a top. High risk of correction. **Example:** BTC at $50k, RSI 75, MFI 85 = everyone bought, possible drop coming soon

### 2. Both Oversold (RSI <30 + MFI <20)

**Meaning:** Low price WITH a lot of money flowing out **Action:** STRONG SIGNAL of bottom. Possible rebound. **Example:** BTC at $38k, RSI 25, MFI 18 = mass panic, buying opportunity

### 3. RSI Overbought but MFI Normal (RSI >70 + MFI 40-60)

**Meaning:** Price rose WITHOUT volume support **Action:** Weak rise, likely FALSE. Do not buy. **Example:** BTC rises 8% but without real volume = bull trap

### 4. RSI Oversold but MFI Normal (RSI <30 + MFI 40-60)

**Meaning:** Price fell WITHOUT real selling conviction **Action:** Weak decline, likely quick rebound. **Example:** BTC falls 7% due to liquidations but without massive selling = recovery soon

## Divergences (Premium Signal)

**Bullish Divergence:**

- RSI makes higher low
- MFI makes higher low
- Price makes lower low = Buy early, bullish reversal likely

**Bearish Divergence:**

- RSI makes lower high
- MFI makes lower high
- Price makes higher high = Sell early, bearish reversal likely

## Practical Strategy

**Buy only when:** RSI <30 AND MFI <20 = Both confirm oversold with volume

**Sell only when:** RSI >70 AND MFI >80 = Both confirm overbought with volume

**Ignore when:** RSI and MFI do not match = Unreliable signal, wait for confirmation

---

# RSI + MFI + TMA + Divergences Indicator

## Overview
Combined momentum indicator displaying RSI, MFI (Money Flow Index), TMA (Triangular Moving Average), and automatic divergence detection for TradingView.

## Key Features

### 1. RSI (Relative Strength Index)
- Default period: 14
- Plotted in yellow
- Overbought: 70+ | Oversold: 30-

### 2. MFI (Money Flow Index)
- Default period: 14
- Plotted in purple (semi-transparent)
- Volume-weighted momentum indicator
- Reference levels: 80 (overbought) / 20 (oversold)

### 3. TMA (Smoothed Moving Average)
- Default period: 50
- Plotted in white
- Acts as dynamic support/resistance for RSI

### 4. Divergence Detection
Automatically identifies four types of divergences:

**Regular Bullish** (green "Bull" label)
- Price: Lower low
- RSI: Higher low
- Signal: Potential upward reversal

**Hidden Bullish** (green "H Bull" label)
- Price: Higher low
- RSI: Lower low
- Signal: Trend continuation upward

**Regular Bearish** (red "Bear" label)
- Price: Higher high
- RSI: Lower high
- Signal: Potential downward reversal

**Hidden Bearish** (red "H Bear" label)
- Price: Lower high
- RSI: Higher high
- Signal: Trend continuation downward

## Settings Groups

**RSI Settings**
- Length and source customisation

**MFI Settings**
- Length and visibility toggle

**TMA Settings**
- Show/hide and length adjustment

**Divergence Settings**
- Enable/disable each divergence type
- Pivot lookback periods (left/right)
- Lookback range (min/max)

**RSI Smoothing**
- Optional additional MA with Bollinger Bands

## Usage Tips
1. Use RSI/MFI together to confirm momentum signals
2. TMA acts as a trend filter (RSI above = bullish bias)
3. Regular divergences signal reversals
4. Hidden divergences signal trend continuations
5. Combine with price action for best results

## Colour Scheme
- RSI: Yellow
- MFI: Purple
- TMA: White
- Bullish signals: Green
- Bearish signals: Red
