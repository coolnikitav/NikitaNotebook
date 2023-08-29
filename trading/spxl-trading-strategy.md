## Disclaimer: This strategy stopped being used on Novermber 25, 2022.

# Background

I have used many technical analysis (TA) strategies to try to gain an edge on the market, which would result in a positive expected value of trades. However, I came across a professional quant on TikTok. He has stated many times that technical analysis does not work, no one uses it in the industry, and has cited studies that show why it doesn’t work. This got me thinking. Many of the books I’ve read and professionals I’ve listened to said that you cannot predict the market or the direction of the market. I have also heard many times that TA uses lagging indicators, so they are not predictive.

# Idea

The main underlying theory of this experiment is that you cannot predict the market. Thus, I thought about taking trades randomly. By taking trades randomly, I have a 50/50 chance of getting the trade right. Thus, there is no advantage (a tiny disadvantage because of the bid-ask spread).

To gain an advantage, I decided to trade the S&P 500, as it has gone up for the past 100 years. I know it is not an indication of it going up forever, but it has been the most stable equity and there will always be top 500 businesses in America. However, trading SPY randomly would not yield returns much better than holding SPY long-term. The capital gains taxes would make the gains even less.

In order to leverage the upside, I decided to trade SPXL – a 3-x leveraged S&P500 ETF.

# Backtesting

The strategy I backtested was: Buy SPXL at the beginning of a trading day. Set a stop loss of 2% and a take profit of 20%. The reason for such a high reward/risk ratio is that I have noticed that most of the profits of SPXL are wiped out by very bad days, where stock drops over 10%. The high reward is because a lot of SPXL gains are made by big runs over 10%. This strategy yielded a 45% CAGR over the last 14 years (since November 2008). This beats the 19% CAGR of long-term holding SPXL and the 10.4% shown by SPY.

# Strategy

Leveraged ETFs perform terribly during huge recessions and crises due to prolonged periods of volatility. Since SPXL was created at the end of the GFC, it has only gone through one crash – the COVID crash of 2020. It fell 78% during the crash. However, it lasted only a couple of weeks. Thus, the leveraged ETF was not affected as severely.

To simulate the performance of SPXL during crashes, I examined the following article: [Simulated Recession](https://seekingalpha.com/article/4291679-spxl-simulated-recession-performance). During the 2008 crash, if you simply held SPXL, you would have lost 96% of your portfolio. During the Dot Com crash, you would have lost 91%. During Black Monday, SPXL went down 61%. And during the great depression, you would have lost 99.8%.

However, let’s examine how our strategy would have performed on some of the worst days of the GFC.

| Date | SPY % change | SPXL % change | My % change |
| :--- | :--- | :--- | :--- |
| October 15, 2008 | -7.7% |  -23.2% | 2%
| October 7, 2008 | -7%| -21% | +6% (due to previous day gains)
| December 1, 2008 | -6.2% | -18.6% | -2% |
| October 9, 2008 | -9% | -27% | -2% |

The strategy protects us from huge intraday losses. This mitigates a lot of the risk of the leveraged ETF and gives us more protection against being wiped out.

# Risks

The current strategy does not protect us from losses that occur outside of market hours. If SPXL drops 15% pre-market, we will lose 15%. Additionally, there is a black swan event where SPY drops 33% in one night and SPXL gets wiped out completely, as well as our portfolio. It has never happened before. However, I am currently reading “Fooled by Randomness” (Check out the book section soon). In the book, the author states that many traders and investors have been wiped out by black swan events.

Currently, I am trying to improve the strategy to give myself protection from such event.
