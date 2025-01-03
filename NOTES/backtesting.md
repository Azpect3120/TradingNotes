# Backtesting and Strategy Creation


### Using the Replay Tool
Using Amazons candle replay tool is a good way to test your strategy.
Allows you to go back in time and see candle by candle.
Can be used to find boxes and use your strategy to find entry and exit points.


### Using a Spread Sheet
You can use a spread sheet to track your trades and see how well your strategy is working.
Columns can include:
- Balance
- Entry Date
- Exit Date
- Symbol
- Setup (boxes, zones)
- Entry (price)
- Stop
- Long or Short (L/S)
- Risk
  - Points (difference between entry and stop)
  - % Risk ((points/entry)*100)
  - $ Risk
- Position
  - % of portfolio
  - Shares
  - $ Value
- Fill
- Exit
  - Exit 1 
  - Size 1
  - Exit 2 
  - Size 2
  - Exit 3
  - Size 3
- MAE (maximum adverse excursion): How much the position works against you before it goes in 
  favor or you take profit. The difference between entry and the point before the positive move.
  This can be written as a percentage. Maybe something like this (((difference = (price-drop))/price)*100)
- MFE (maximum favorable excursion): How much the position went in your favor before you exited.
  Can tell you the max possible profit from the position. This can tell you if you need to exit
  sooner. The maximum value the price reached before the exit.
- TS
- Reward
  - Points (exit-entry)
  - % Reward
  - $ Reward
  - Days in Trade
