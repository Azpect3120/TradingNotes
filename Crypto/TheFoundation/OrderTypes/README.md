# Order Types

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
