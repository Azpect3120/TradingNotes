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


