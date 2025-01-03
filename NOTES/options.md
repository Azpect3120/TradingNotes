# Options or Stock Options


## Overview
A financial instrument that gives its owner the right, but not the obligation,
to purchase a given asset at an agreed-upon price and date.

An added layer onto a future. Allowing one party to back out of the deal, the 
other party is paid a **premium** for allowing the other party to make this choice.

- Like futures, their price is derived from the price of an underlying asset.
- Maximum leverage while capping your losses/risk.
- Slightly more complicated.
- Heavily affected by market events.

### The Premium
In order to have this privilege, the buyer pays a fee to the seller. This is called 
the **premium**.


### Terms & values
**Intrinsic Value**: The value of the option if it were to expire immediately (today).
- Formula: (Share price in the market) - (strike price)

**Extrinsic Value**: The time value, the value we assign to it. Time allows the price 
to move in the direction we want it to.


### Two Types of Options
**Calls**: Allows the buyer to to purchase a specific amount of the underlying asset 
from the seller at the strike price at expiration.

- **Increases** in value as price goes **up**.
- Intrinsic value + Extrinsic value.

**Puts**: Allows the buyer to sell a specific amount of the underlying asset to the
seller at the strike price at expiration.

- **Increases** in value as price goes **down**.
- Intrinsic value + Extrinsic value.


### Definition
Defined by **underlying, expiration date, and strike price**.

**e.g.**: `$AAPL Aug 20 $100 call`


### Options Price?
The price of the option (premium) is determined by the price of the **underlying asset**, 
the **time until expiration**, and the **implied volatility** of the underlying asset.

The option who's strike price is closest to the current price of the underlying asset
is more expensive than the others. This is because it takes longer for an option to make 
profit the farther away it is from the current price. A put for example, has to move farther
downward in order to make profit.


### Player vs Casino
- Buyer of options pays premium.
- Seller of the options receives premium.
- Think of the premium as the fees required to enjoy the luxury of owning an option.

Max profit from the buyer's perspective is unlimited (within reason), while the max 
loss is the premium.

Max loss from the seller's perspective is unlimited (within reason), while the max 
profit is the premium.


### Spreads
A position that consists of two or more options of the same type.
Two or more calls or puts.

#### Bull Call Spread
- Created when you expect bullish price action.
- Buy a call with strike *A* and sell with a strike *B* where *B* > *A*.
- Premium paid.

This is done to reduce the cost of the premium, while still having the potential to
make a profit.

Basically, you are buying a call option at 40$ (for example) and selling a call option
at 45$ (for example). This way, as long as the price is above 42$, the winnings made 
from the 40$ call will cover the losses of the 45$ call. This will *somehow* reduce the
premium paid.


#### Bull Put Spread
- Created when you expect bullish price action.
- Buy a put with strike *A* and sell a put with strike *B* where *B* > *A*.
- Premium received.

Selling a more expensive option, and buying a cheaper option. This way, you are
reducing the losses.

Goal is to have the options expire worthless.


#### Bear Put Spread
- Created when you expect bearing price action.
- Buy a put with strike *A* and sell a put with strike *B* where *A* > *B*.
- Premium paid.


#### Bear Call Spread
- Created when you expect bearing price action.
- Buy a call with strike *A* and sell a call with strike *B* when *A* > *B*.
- Premium received.

Goal is to have the options expire worthless.


## Straddles and Strangles

#### Straddle
- Expectation of a large move but no dias on direction
- Buy a call and put with the same strike price and expiration date.
- Bottom straddle vs top straddle.

The only way to lose is if the price does not move at all. The more the price moves,
the more you win. As long as the move is significant enough to cover the premium of 
each option.


#### Strangle
- Expectation of a large move but no bias on direction.
- Buy a call and put with different strikes and same expiration date.
- Lower risk than straddle. Price has to move farther than straddle for profit.

Spending less on the premium, but the price has to move farther in order to make
a profit.

The zone between the two strikes is the zone where you lose the most money. If the 
call expires less and the put expires more, you lose the most money. That is the zone.

The move that happens needs to be bigger than what the market was expecting.


## Butterflies
- Expectation of price to be range bound.
- Buy a call with strike *A*, sell two calls with strike *B*, and buy a call with
strike *C* where *A* < *B* < *C*.

The calls that you buy, envelop the calls that you sell. As long as price stays within
the strike of the calls you buy, the calls you sell with expire worthless and the calls 
you buy will make a profit. If price leaves the range, you will end up with a loss.


## Iron Condors
- Expectation of price to be range bound.
- Combination of a bull put spread and bear call spread.
- Premium received.

You are expecting the price to stay within a certain range.

Capped losses and capped winnings. The winnings are based on the premium received 
from the bull put spread and bear call spread.

Typically a better option compared to butterflies.


## The Greeks

### Delta
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


### Theta 
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


### Gamma
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


### Vega
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


## Risk in Options vs CFDs
- Higher leverage = higher risk = higher winnings & higher losses (CFDs).
- The lowest an option can go is 0, while CFDs can go negative.
- An option working against you, can only hit 0, the maximum loss is the amount
  you put in.


### How to use CFDs
- Prefer swings over scalps.
- Never hold them through earnings.
- Never hold a scalp overnight.
- Trade assets that are available 24 hours such as US500 and US100.


### How to Sell Premiums
- Selling premiums in low volume conditions is not good. Choppy is fine but low volume
  conditions are not.

##### e.g. #1: Price is breaking out of a 50DMA box after a large base box. Price is about *$530*

What do you do?
- Buy calls and go long (what most people do, what we do)
- Sell premium

How do we **sell premium**?
- We sell a put at *$524*
- We buy a put at *$518*

Why?
- Options closer to the current price are more expensive, which means when we sell an expensive
  option and buy a cheaper option, we are making profits from the difference in premium.
- What we just did, is create a **bull put spread**.
  - We are expecting the price to go up.

What happens if the price is choppy and does not go up right away?
- Nothing! It is okay! Because **theta** is working in our favor, the puts are losing value
  as we approach the expiration date.
- Which means: When we buy back the put we sold, it will be cheaper than what we sold it for.
- If they do not move at all, the puts expire worthless and we keep the premium we received!

What happens if the price goes up?
- The puts will expire worthless and we keep the premium we received at the beginning!

What happens if the price goes down?
- You will lose money, so we will use a stop loss to prevent further losses. As long as the 
  price stays above the put we sold, the options will expire and lose value over time.


##### e.g. #2: Falling 50DMA and price is breaking lower. Price is about  *$430*
*note: less information will be provided here*

What do you do?
- Put long puts (if we are unsure about the strength, this could be a bad idea!)
- Sell premium (we will use a bear call spread)

How do we place a **bear call spread**? 
- Sell a call at *$438*
- Buy a call at *$445*

Why?
- We are expecting the price to go down and the calls to expire worthless.
- As long as the price is bellow the *$438* area, we will make a profit!
- Upon buying, the premium will be our profits!

Outcome:
- Price is chopping around: We will make profits from the theta decay. As long as the price 
  stays below *$438*, we will make profits.
- Price goes down: Same as before in e.g. #1, we will make profits.
- Price goes up: We will lose money if price crosses *$438*. We will use a stop loss to prevent
  further losses.

What if we don't know that direction the price will take?
- We can use a **bear call spread** and a **bull put spread** at the same time. 
- This way, we  will make profits as long as the price stays within the range of the two spreads.
- This is called an **iron condor**.

##### Why are we doing this? Why not just sell the expensive option?
- It can be hard to get permission from the broker to do this (level 4 permissions).
- If the price goes against us, we can lose a LOT of money (unlimited losses).
- The cheaper puts that we bought will prevent losses from the puts we sold if the price 
  drops like a rock. 
- Prevents huge losses if something drastic happens.
- The maximum risk in a spread is the difference between the two strikes. The maximum 
  risk in a single option is the premium paid. OR if you are just selling a single option,
  the maximum risk is unlimited.

##### More notes
- Prof will typically sell out at 70%. There is no need to hold the options until expiration 
  if the price moves in your favor.
- If the price is chopping it can be hard to know when to sell and you may need to hold longer 
  and wait for the theta decay to work in your favor.
- Ideally you want to use limit orders to sell the options at a certain price. This way you 
  can set it and forget it. Market orders can make it difficult



### Calculations on Spreads
- All spreads and options should be calculated with a single contract.
- Options are all prices in hundreds. So $1.54 is actually $154.
- However, calculations should be done in their single increments, not hundreds.

When buying a spread the maximum profit is the difference between the premiums of the two and
can be calculated using this formula:
`A: premium of the option you sold, the expensive one`
`B: premium of the option you bought, the cheap one`

##### Maximum profit per contract: `A - B`

e.g.:
- Premium of A: $1.54 (a piece)
- Premium of B: $0.44 (a piece)
- Maximum profit: $1.54 - $0.44 = **$1.10** (a piece)


The maximum loss can be determined using this formula:
`D: difference between the strike prices of the options you bought and sold`
`A: price of the option you sold, the expensive one ($154 is equal to 1.54 since options are 
counted in hundreds)`
`B: price of the option you bought, the cheap one ($44 is equal to 0.44 since options are 
counted in hundreds)`

##### Maximum loss per contract: `D - (A - B)`

e.g.:
- Strike price A: $538 (sold)
- Strike price B: $533 (bought)
- Difference between A and B: $5
- Option price A: $1.54 (a piece)
- Option price B: $0.44 (a piece)
- Maximum loss: $5 - ($1.54 - $0.44) = **$3.90**


The formula to calculate the break even point is:
`S: strike price of expensive option (the old you sold)`
`A: price of the option you sold, the expensive one ($154 is equal to 1.54 since options are 
counted in hundreds)`
`B: price of the option you bought, the cheap one ($44 is equal to 0.44 since options are 
counted in hundreds)`

##### Break even price point: `S - (A - B)`

e.g.:
- Strike price A: $538
- Option price A: $1.54 (a piece)
- Option price B: $0.44 (a piece)
- Break even point: $538 - ($1.54 - $0.44) = **$536.90**

