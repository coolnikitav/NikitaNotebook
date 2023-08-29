# Reducing Risk of The SPXL Trading Strategy

## Results 
### Disclaimer: This strategy stopped being used on November 25, 2022.

The strategy has been running for about two month. The results are displayed below.

![image](https://github.com/coolnikitav/nikitas-notebook/assets/30304422/09f9c872-ef80-4532-ada5-08860f565370)

Since September 7, my strategy has had a return of 3.69%. The return is not compounded, every trade is made with $8000. Holding SPY over the same period would have resulted in a 2.08% return. Holding SPXL would have returned 0.55%.

Return of the SPXL daily trades is 10.69%. However, the put is sitting at a $555 loss. This brings the return down drastically.

I think that this strategy does a great job of cutting losers early. However, it does not do a good job of taking big profits. In addition, I do not think that a put is necessary, since an overwhelming majority of the trades close before market close.

## Background

As mentioned in the previous post about this strategy, black swan events occasionally occur and wipe out many traders and investors. My SPXL strategy would fail if S&P500 drops 33% in a single night. Not probable, but possible (it has dropped 22.6% in a day before). It would also suffer huge losses if the market fell less, but for a longer period. This often happens to leveraged ETFs. They would be up significantly for years and then lose 95% in a single drop.

## Idea

The article I mentioned in the previous post: Simulated Recession, discusses purchasing puts to protect myself from a rare crash that would typically wipe out 95% of the value of the ETF. Another factor that would increase the value of the put is volatility. During huge crashes, volatility typically rises and options become more valuable.

The put decreases future profits by the value of the put. However, it is necessary to protect the position from the rare negative events.

## Payout Analysis

The following payoff table is for purchasing 130 shares of SPXL for $8000 and holding it. If the price doubles to $124, we double our money and secure a $8000 profit. If the price drops to 0$ we lose the entire $8000 amount.

*Payoff table for 130 shares of SPXL at $62.66*
![image](https://github.com/coolnikitav/nikitas-notebook/assets/30304422/3200b13e-9231-4438-92a9-8583d5705c20)

The following payoff table is for purchasing 130 shares of SPXL for $130 and a 20 Jan 2023 60 Put for $835. If the price of SPXL doubles, we profit roughly the same amount. Our profit is 10% less because our put become worthless ($835 of $8000 is about 10%). Now, if the ETF plummets, we only lose up up to $3000. The loss is 63% less than before. This is a huge difference, as the account is not blown up and we are ready to invest at market lows.

*Payoff table for 130 shares of SPXL at $62.66 and a 20 Jan 2023 60 Put for $835*
![image](https://github.com/coolnikitav/nikitas-notebook/assets/30304422/c8cbb6e7-9035-4eaf-9972-30a6d98e53bf)

## Risks
The strategy involving the put does underperform when the price is above $52 ($60-$8.35). However, it underperforms only by about 10%.

In addition, the payoff tables do not fully depict the SPXL strategy I am using. The strategy shown is for buying and holding SPXL. On the other hand, I am trading it daily with a stop loss. It is difficult to show projections for my strategy. However, generally, when the ETF is going up, my strategy would be making money. And when the ETF is going down, it would be losing it.
