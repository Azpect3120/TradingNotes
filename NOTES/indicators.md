# Stock Market Indicators


### Simple Moving Average (SMA)

It displays the average price of a stock over a period of time. The **length** of the
duration is determined by the length of the input and the tables current settings.
Eg. a length of 9 in a 1 hour chart will display the average price of the stock over
the last 9 hours. 

##### Some example usages:

- If the average of the stock over the last 50 days is raising, it is a medium term
bullish(up) signal.


### Squeeze Pro (sqzpro)

The dots in the center line of the indicator represent the tightness of the contraction
of the stock and therefore the how big the expansion will be.

Based on the Boligner Bands and Keltner Channels.
- The BB measures information based on daily closes
- The KC measures information based on daily highs and lows (defines volatility based on gap 
  between highs and lows)

If the bands are tight, it means the market did not move much. However, if the market moves high 
and then low but closes at the same(ish) price, the channels will notice this and show high 
volatility.

##### How to read the indicator:

**The dots:**
- Green dot: no consolidation
- Orange dot: mild consolidation (his are black)
- Red dot: tight consolidation
- Yellow dot: no consolidation but some volatility

**Green dots** are a good indicator of **no contraction** and **no boxes**.
**Orange dots** can be a good indicator of a **contraction**.
**Red dots** will be stronger than orange dots and will create a **stronger box** you can trade from.
**Yellow dots** will create the **tightest box** you will see and a very **strong contraction**.

The **tighter** the box, the **stronger** the move will be.
This indicator should be used as a **screener** to find boxes or prove boxes.


### RSI
Relative Strength Index (RSI) is used to assess the strength/momentum of a movement. Goes from 
0 to 100. Most people define overbought as 70 and oversold as 30. However, this does not always rain 
true. Just because the RSI crosses 70 or 30, it does not indicate a reversal. At those points we should
look for divergence.

The other line (base MA) is the moving average of the RSI. When the RSI is above the base MA, it is
considered bullish momentum. When it is below, it is considered bearish momentum.

##### Size
- **14** is the most common size
- **5** could be used for scalping

##### Divergences
- **Bullish**: When the price is making lower lows but the RSI is not.
- **Bearish**: When the price is making higher highs but the RSI is not.

- **Hidden**: When the RSI is making higher highs but the price is not and vise versa.
  Much less common but they do occur, the market usually loses hope in the move and reverses.

Divergences are a good indicator of a slowing momentum and a possible reversal.
**Much stronger** sign compared to oversold or overbought signals.

##### The Momentum Average Convergence Divergence (MACD)
Works very similar to the RSI, the 0 line is the average and values above are bullish and below are 
bearish. They are used the same way even though their calculations are different. Using the MACD and
the RSI is a bit redundant.


### Fibonacci Retracement
This is not an indicator but a tool to find levels of support and resistance. It is based on the 
fibonacci sequence. It can be used to find levels for retracement in a trend; levels where the price
maybe find support or resistance. The values Prof uses are 0.382, 0.5, and 0.618. They can be good
to place stop loses and take profits, or used to find locations to enter or add to a trade.
