# Crypto

## Terms

**Fiat Currency:** Currencies that have value because they are minted 
by a central bank. Examples include USD, GBP, EUR.


## Spot vs Perpetual Futures

**Spot:** Exchanging fiat current for crypto currency or another 
crypto currency for another at the current market price. You receive
and own the action coin.

**Perpetual Futures (Perps):** A derivative contract that allows you to
speculate on the future price of a coin without actually owning it. Offers
margin (leverage), which means you open a position with a fraction of the 
price (similar to options).

These function similarly to the way options v. equity works. Long term 
investments should be made in a spot market, while short term investments
should be made in a futures market.

## CEX vs DEX

**CEX (Centralized Exchange):** When you give your money to these exchanges,
it is no longer your money, until you withdrawal it. Examples include, 
Binance, Bybit, bitMEX, OKX and Kucoin.

**DEX (Decentralized Exchange):** You connect a wallet to this kind of exchange,
which allows you to store the coins you purchase. Examples include GMX. A 
safe option because your money is not at risk of being stolen by the exchange
or a malfunction.

## Order Types

#### Standard Orders

Same orders as we use in the stock market. **Market**, **limit** , Stop, TP, and
Trailing stop.

#### Advanced Orders

Same as the ones we use in trading but I will detail them here.

**Stop-Limit Order:** A stop order that does not execute as a market order, but
as a limit order. Contains the same risk as a limit order.

**Immediate or Cancel (IOC) Order:** An order to buy or sell a token immediately, 
but any portion of the order that cannot be filled immediately is canceled.

**Fill or Kill (FOK) Order:** An order to buy or sell a coin that must be filled
in its entirety immediately, or canceled if it cannot be.

**Good til Canceled (GTC):** An order which will remain open until it is either
executed or canceled.

#### Conditions

**Reduce Only:** Selecting this along with your order will ensure that only an 
existing position can be reduced and a new position cannot be opened in the 
opposite direction. Best practice is to always select this for stop losses.

**Post Only:** Selecting this with your order will only execute if it would 
result in adding liquidity to the order book ('maker' or 'limit' order). Just 
ignore this, its not very important.


## Leverage

#### Terms

**Collateral:** Asserts that act as a form of sectary to cover potential losses.

**Margin:** Amount of collateral that you must hold to cover potential losses.

**Initial Margin (Cost):** Amount of collateral required to open a position in perpetual
futures trading.

**Maintenance Margin (MMR):** The minimum amount of collateral you must hold to keep a position 
open. Differs from exchange to exchange, as well as coin to coin.

**Notional Size (Value):** The total $ value of your position. Notional Size ($) = Number of 
coins **x** current price of 1 coin. Changes in real time.

**When losses exceed maintenance margin, you will be liquidated.**

**MMR is a % of the Notional size of your position.**

**Leverage:** The amount you need to borrow from the exchange **AFTER** you known your entry,
stop loss, and notional position size.

***Leverage Comes Last.*** Doesn't matter how much leverage you use, it matters how much money 
you risk on  each trade. If you have $1000 and want to risk 1%, your stop loss should be set 
to lose $10, regardless of leverage. Leverage required will be different for each trade.

**Position Size Calculation:** Risk ($) / Entry - Stop Loss

e.g. You want to risk $10 (1% of portfolio) on an ATOM Long trade. Entry = $10.60 & Stop Loss = 
$10.10. So... **$10 / $0.50 = 20 ATOM**. Notional = 20 ATOM x 10.60 = $212. Leverage is the amount
you need to borrow from the exchange to open a $212 position.
