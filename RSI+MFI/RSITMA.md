
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
