# The Greeks

## Delta
Rate of change of option price with respect to the underlying asset.
The *delta* value is amount an option's price would change if the underlying stock 
changes by $1.

Delta has no units, it is a ratio.

Delta can be **thought** of a probability of the option expiring in the money.

Eg. If the delta of a call is 0.5, and the call is priced at $2, if the stock goes up 
by $1, the call will be priced at $2.5.

= $2 + (0.5 * $1) = $2.5

##### Key Terms
- **ITM**: In the money.
- **ATM**: At the money.
- **OTM**: Out of the money.

##### Call Deltas
- Positive.
- Positive correlation to underlying price change.
- Range from 0 to 1.

##### Put Deltas
- Negative.
- Negative correlation to underlying price change.
- Range from 0 to -1.

##### Delta vs Time & Volatility
- Delta => Probability of option expiring ITM.
- As options get closer to expiry, ITM delta moves toward 1 (or -1, for puts) and OTM deltas moves toward 0.
- As implied volatility increases, delta of options shifts towards 0.5.


## Theta 
Rate of change in the option price with respect to the time left till expiration.
The theta value is the mount an option's price will decline per day while all the 
other factors remain constant. Pricing models take weekends into account.

There is no standardized way to calculate theta.

Causes the extrinsic value to decrease as the expiration date approaches.

Options lose value as time goes on.

##### Theta Decay
- Theta is always negative.
- The theta decay is non-linear.

##### ITM vs ATM vs OTM
Theta is highest for options ATM closer to expiration and highest for far OTM 
options furthest from expiration.

- ATM options lose the most value as they approach expiration.
- OTM (far) options lose the most value the farther out the expiration date is.

Most of an OTM option's extrinsic value is lost, the farther out the expiration 
date is.

##### Theta vs Volatility
Theta increases as volatility increases. This is because as time goes on, a more
volatile stock is more likely to move in the direction you want it to. This is
why the theta is higher for options with higher volatility.

Extrinsic value drops more over time for options with higher volatility.


## Gamma
Rate of change of option delta with respect to the underlying asset price. The 
relationship of option price wit change in underlying asset price is not linear.
For this reason, delta hedged portfolios need to keep strict track of gamma as it 
becomes significant if a large move in underlying occurs.

How much delta changes with a change in the underlying asset's price. Gamma is the 
slope of the delta curve.

To prevent your portfolio from becoming unbalanced, you need to keep track of gamma.

##### ITM vs ATM vs OTM
- Generally has its peak value close to ATM.
- Decreases as the option goes deeper ITM or OTM.

##### Gamma vs Time
Gamma is smoother for options with higher time to expiration.

As time to expiration decreases, gamma of ATM options increases while those of OTM and 
ITM options decreases.

##### Gamma Squeeze
Market Makes delta neutral portfolio. Near expiration, delta prices can change fast 
especially around spot price. That needs constant hedging and can lead to loops of 
extreme price movements.

The market makers will have to buy more shares to hedge their position, which will 
cause the price to go up. This will cause more people to purchase calls and the cycle
will continue and can eventually become overwhelming. These abrupt price movements 
are known as gamma squeezes.


## Vega
Vega measures the change in option price based on a 1% change in the underlying asset's
implied volatility. IV (implied volatility) is a measure of predicted future movement.
IV has no direct correlation to historical volatility. IV is calculated using current 
market premiums. Vega is **always positive**.

Does not really affect how we buy or sell options, but keep in mind that options will 
cost more when big events, like earnings, CPI, or FOMC, are coming up.

##### ITM vs ATM vs OTM
- Highest for ATM options.
- Tends to zero for ITM (far) and OTM (far) options.

##### Vega vs Volatility
- Higher the volatility, the flatter the Vega curve will be.
- In high volume conditions, the ATM point is less rigid.

##### Vega vs Time (DTE, Days to Expiration)
- Vega impact dies out as get closer to expiration.
- The exact opposite of gamma.
- The farther away the option is from ATM, the quicker Vega impact will die out with time.
