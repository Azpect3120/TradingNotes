# Math of Profitability

Expected Value (EV): Weighted average of the possible values of a variable. In our case, PnL.
- EV = Prob.(win) * reward + Prob.(loss) * risk

### Reward to Risk Ratio (RRR)

`Reward`: Amount you make on the trade

`Risk`: Amount you risk losing on the trade

To calculate minimum winrate in order to be BE:

- 0 = P(win) * reward + P(loss) * risk
- 0 = P(win) * reward + [1 - P(win)] * risk
- P(win) = 1 / [1 + (reward / risk)] = **1 / (1 + RRR)**

![Minimum Winrate Chart](https://github.com/Azpect3120/TradingNotes/blob/master/Stocks/SuperchargeYourProgress/PsychologyAndMindset/MathOfProfitability/minWinRatePerRRR.png)

### Mindset Adjustments

- Backtest your system to determine its win rate and RRR
- Log your trades to see if practical win rate and RRR is the same as the backtest
- Adapt a system whose win rate will align with your personailty
