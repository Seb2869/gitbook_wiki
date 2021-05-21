# Interest rate guide

[https://www.investopedia.com/personal-finance/apr-apy-bank-hopes-cant-tell-difference/](https://www.investopedia.com/personal-finance/apr-apy-bank-hopes-cant-tell-difference/)

[https://en.wikipedia.org/wiki/Rate\_of\_return](https://en.wikipedia.org/wiki/Rate_of_return#Annualisation)

Let's describe this logic step-by-step for yield farming strategies.

For example, you have $1000 `A` and invested it in strategy `X`

### Strategy profit

Strategy `X` puts your asset in a project `pX` with standard Harvest logic \(periodically claims rewards and adds them back to the project\)

Project `pX` has $**1M** TVL `pTVL` and $100,000 of rewards `pReward` that will be provided over a 30 day period `pPeriod`

Your $1000 is 0.1% of the Total Value Locked \(TVL\) `A / pTVL`

This means your asset will receive $100 during the month `pReward * (A/pTVL)`

In DeFi when comparing profits, most projects show APR, but call it the APY.

For example, you can multiply your monthly profit for 12 months of the year and get an annual profit figure.

Of course, 12 months with the same profit and TVL is an unrealistic situation. Let's call this the "Instant APR" `iAPR` , because it is the APR for the current situation and will change as TVL and rewards change.

For your $1000 it will be \( `pReward * (A/pTVL)`\* 12 = $1200\) ⇒ $1000 / $1200 = 120% `APR`

But your asset is under the strategy's control. It claims profit every day and adds it back into the project. In this way, it generates additional profit the longer you hold it, due to the principal of compounding returns.

Daily profit will be `pReward` /`pPeriod` = $100,000 / 30 = $3333.33.

For your share of 0.1% it will be $3.30 per day.

So after the first day your total stake will be $1003.30.

Your new share % will be $1003.30 / $1M = 0.1003%

For day 2 you will receive $3.44, due to the compounding effect from day 1. Each day thereafter, your daily profit will continue to increase.

Your final compounded annual profit is the APY, but don't forget the project only has rewards for the month!

APY is calculated for the year so that we can compare different projects with different periods of work.

Let's call it instant APY or `iAPY`

The formula for APY calculation is a bit complex:

![](../../../.gitbook/assets/image%20%288%29.png)

\(Math.pow\(1.0 + \(\(apr / 100\) / period\), period\) - 1.0\) \* 100

For 120% `iAPR` it will be 231.36% `iAPY`

For most strategies, Harvest Finance has a rule that 70% of profits go directly to stakers, with the remaining 30% going to FARM buyback. Remember to include this when calculating final APY%.

### Weekly FARM reward

Every week Harvest Finance mint FARM tokens and send it to the stake contracts. The amount of FARM tokens minted decreases each week by 4.44%.

For traditional stake contracts \(not AutoStake\), it means that each new 7 day period of rewards start with this FARM amount.

This provides additional yield for each strategy. Calculate it with the same rule and add to the final APY%.

