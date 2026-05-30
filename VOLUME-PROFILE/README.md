<img width="1309" height="1001" alt="image" src="https://github.com/user-attachments/assets/8dfc7382-ca73-4603-b629-3fc501edcccc" />

# Volume Profile ULTRA Precise

## Function
Indicator track volume at price. 
Reset every day 00:00 UTC. 
Use 1-minute data. Much precise.

## Visuals
* **White Line:** Point of Control (POC). Most volume traded here.
* **Orange Dashed:** Value Area High (VAH) and Low (VAL).
* **Bright Bars:** Value Area. Where % volume goal lives.
* **Green vs Purple:** Split buy volume vs sell volume.

## Inputs
* **Row Size:** Number of price buckets. More rows = more detail.
* **Value Area %:** Volume goal for highlight. Default 70%.

## Technical Limits
TradingView limit 500 boxes total.
Calculation: `Rows` x `2` x `Days` = `Total Boxes`.
Too many rows make old days disappear. 
Lower "Row size" to see more history.
