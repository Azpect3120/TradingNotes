# Spreads
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

## Calculations on Spreads
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

