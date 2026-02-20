# Market Profile — Performance and Stability Fixes (Pine Script v5)

This repository contains a modified version of the original [Market Profile](https://github.com/agejevasv/tradingview/blob/main/marketprofile.pine) indicator with critical performance optimizations and runtime stability fixes for Pine Script v5.

Special thanks to [Viktoras Agejevas](https://github.com/agejevasv) for the original implementation.

## Overview

These modifications resolve the common runtime error:

```

Loop takes too long to execute (> 500 ms)

````

and address additional issues including:

- Index out-of-bounds errors  
- Boolean type mismatch warnings  
- Ticker ID inconsistencies  
- Inefficient volume profile calculations  

The result is a significantly faster and more reliable Volume Profile POC calculation.

## Key Improvements

### 1. Volume Profile Performance Optimization

Replaced expensive array searches (`array.indexof`) with direct index mapping using mathematical calculation:

- Converts O(n) search operations into O(1) direct access
- Uses a fixed-size volume buffer (`vol_buffer`) for efficient memory usage
- Eliminates dynamic array growth inside loops
- Improves performance by approximately 50–100×

This prevents Pine Script’s 500 ms execution timeout.

### 2. Index Safety Fixes

Resolved out-of-bounds errors by:

- Using `math.floor` instead of `math.round`
- Clamping indices between valid bounds (`0` to `size - 1`)

This ensures safe array access under all conditions.

### 3. Pine Script v5 Type Safety Compliance

Fixed boolean and `na` handling by replacing implicit checks with explicit comparisons:

- Replaced invalid boolean coercion with `not na(...)`
- Ensures compatibility with Pine Script v5/v6 strict typing

### 4. Correct Ticker Reference

Replaced:

```pine
syminfo.ticker
````

with:

```pine
syminfo.tickerid
```

This ensures accurate data retrieval across exchanges and adjusted symbols.

## Result

These fixes provide:

* Stable execution without timeout errors
* Faster Volume Profile and POC calculations
* Improved memory efficiency
* Full Pine Script v5 compatibility
* More reliable multi-timeframe behavior

## Credits

Original Market Profile implementation:
[https://github.com/agejevasv/tradingview/blob/main/marketprofile.pine](https://github.com/agejevasv/tradingview/blob/main/marketprofile.pine)

Modifications focused on performance optimization and runtime stability.
