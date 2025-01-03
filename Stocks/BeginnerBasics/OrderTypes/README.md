# Order Types


## Bid - Spread Ask

- Bid: Highest price a buyer is willing to pay.
- Ask: Lowest price a seller is willing to accept.
- Spread: Difference between the bid and ask.

Smaller spread means there is more liquidity in the market, due to more 
buyers and sellers.


## Limit Order (LMT)

An order to **buy or sell a stock at a specified** price or better.

- **Buy at or below** the bid price.
- **Sell at or above** the ask price.

If you place a limit order to buy a share at $50, and the current price is 
less than $50 (eg. $45), the order will be executed at the current price (eg. $45).
If a limit order is placed at a point in which the market never reaches, the order
will not be filled. They do not have to execute immediately.


## Market Order (MKT)

**Immediately buy** at the lowest ask price or **immediately sell** at the highest 
bid price.

Used for an **immediate in liquid markets** because it will get filled right away.

- Should only be used when the market is **liquid**.
- Should only be used when the **spread is small**.

If an attempt to buy 1000 shares of a stock is made at market value, but only 500 
shares are being sold at market value, **SOMETHING WILL HAPPEN BUT IT MIGHT NOT 
LET YOU DO THAT**


## Stop/Stop Market Order (STP)

Once **stop price is hit, a market order is sent** to close out your trade.

Risk: **your trade is closed extremely from from your intended price** in case 
of a massive gap up/down. If a market opens or closes at a gap up/down, the 
stop price will be hit and the market order will be sent.

Allows your to place a **stop loss** on a trade to prevent further losses.


## Stop Limit Order (STP LMT)

Once stop price is hit, **a limit order to close your trade** will be placed
at a pre-specified price.

Risk: Your **limit order never gets hit**

If you place a stop limit order to sell a stock when a certain point is reached,
but you set the limit price too high, the stock may never reach that price and
the order will not be filled. Therefore, you will still own the stock and the
price will have dropped.
