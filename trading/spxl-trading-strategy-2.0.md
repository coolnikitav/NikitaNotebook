# Results (as of Feb 7, 2023)
I started using this strategy on October 19. The results are displayed below.

![image](https://github.com/coolnikitav/nikitas-notebook/assets/30304422/fba403b7-3d10-4940-afd6-c2d8f6c85f82)

Since October 19, the SPXL strategy has had a return of 34.01%, tripling the return of SPY and beating SPXL itself. There were 75 trades: 49 wins averaging a 2.25% gain and 35 losses averaging a 1.69% loss.

Strategy is close to the target return of gains (2.5%) and losses (-1.5%). It has underperformed SPXL during positive months and outperformed during negative ones. Risk management is extremely important, since big losses are worse than big wins. Thus, the strategy is working as expected.

# Background
SPXL Trading Strategy 1.0 was started at the beginning of September 2022. After about a month of testing, I noticed its flaws.

First of all, the put used to protect the account from a black swan event was losing a lot of value when the market was going up. An overwhelming majority of the time position is sold before the market close. Thus, the chance of a position staying open overnight AND a giant drop in the market is extremely low. So low that it is not worth losing money on the protective put.

Second, the strategy was not good at capturing profits. Since the only part of the trade was a 2% trailing stop loss, most trades ended with a small profit or a medium loss.

# Strategy
The new strategy includes entering a long trade on SPXL at the beginning of each day, setting a 3% trailing stop loss, a 3% take profit goal, and doing a simple market sell at the end of the day if neither the stop loss nor the take profit is reached.

# Strengths
SPXL Trading Strategy 2.0 has all characteristics of a profitable trader. It lets profits run until the profit target, cuts losses short, and keeps losses small (3% max).

# Weaknesses
The strategy operates under the assumption that the S&P500 will keep growing in the future. If S&P500 doesn’t go up, it is practically impossible for this strategy to make money.

# Expectations
The expected loss is around 1.5% – half of the stop loss. There is a 3% trailing stop loss. However, it is very rare for the market to open and just nose-dive. It usually goes up, moving the stop loss up.

The expected profit is 2.5%. There is a 3% profit target. However, sometimes volatility in the market is low and it doesn’t move much, not reaching either target and resulting in a market sell. This brings the expected profit from 3% to 2.5%.
