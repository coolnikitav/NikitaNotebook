# Background

I began using the second version of my trading strategy on October 19, 2022. I traded SPXL at first, but switched to SPY in April 2023. SPY has greater liquidity than SPXL, making it easier to enter and exit trades. I used 3x leverage on SPY to simulate the SPXL trades. After 6.5 months of trading, the strategy has proven to be quite successful. However, I found that it can be optimized based on past performance.

I have taken 132 trades since October 19. Each trade generated between -3% and 3%. 43 out of the 132 trades yielded between 2% and 3%. I noticed that during 37 out of 43 (86%) of these trades, the stock price rose immediately and continued to rise until reaching the target profit. During those trades, the stock did not dip more than .5% (1.5% loss) before reaching a profit of 2%-3%.

Losses can be reduced while keeping 86% of the big winners by cutting the stop loss in half: from 3% to 1.5%. My risk tolerance allows for a 2% loss per trade. Thus, I will use 4x leverage to bring the stop loss to 2% and take profit to 4%.

I am confident that this optimization will further improve the performance of my trading strategy. I will continue to monitor the results and make adjustments as needed.

# Strategy

The new strategy is similar to the previous version. Long SPY in the beginning of the trading day with 4x leverage. Set take profit to 1% (4% with leverage). Set stop loss to 0.5% (2% with leverage). Then set a trailing stop loss of 1% to make sure we do not lose all of the profits when the stock rises fast.

# Strength

The main strength of this strategy is keeping an overwhelming majority of the big winners, while reducing losses.

# Weakness

The main weakness of this strategy remains the same: it relies on SPY growing over time, which relies on the US growing over time.

The weakness of this version of the strategy is a greater number of losses. The stop loss is smaller, thus, there will be more losses. However, they should be small.
