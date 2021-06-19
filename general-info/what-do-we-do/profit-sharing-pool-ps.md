---
description: The distribution of protocol fees to FARM-holding investors.
---

# Profit Sharing and iFARM

### Profit Sharing

![](../../.gitbook/assets/ps1.jpg)

A key innovation of the `$FARM` token is that it entitles holders to a performance fee \(**currently 30% ETH and 8% BSC**\) taken from Harvest's yield farming strategies. While each strategy may farm different assets, the performance fee is used to buy `$FARM` on the open market, which is then distributed to those who stake `$FARM` in the Profit Sharing pool. The price of `$FARM` is subject to consistent buy pressure as a result. To participate, users must first obtain FARM by collecting incentives for participating in Harvest's yield farming pools, or simply buying FARM directly on the open market. Then FARM must be staked in the auto-compounding Profit Sharing pool.

### Technical Details

The profit sharing pool is a modified SNX style staking pool. Once FARM is purchased on the open market it is distributed pro rata per second to all those staked in the Profit Sharing pool over a duration of 1 day, with each new reward added resetting the duration of the payout. As a result, the instantaneous reward rate for the Profit Sharing pool fluctuates over the course of the day. For this reason, a 7-day average of the reward rate is displayed for this pool. The instantaneous rate can always be checked by reading the contract directly.

### Auto Compounding

In order to rectify the observation that the FARM reward token given to our users needed to be regularly be claimed and restaked in Profit Sharing, we added an auto compounding function to the Profit Sharing pool. Whenever _any_ user deposits or withdraws funds from the Profit  Sharing pool, the rewards for _all users_ are automatically collected and restaked to improve their returns and save long term stakers gas. While this increased the cost associated with staking FARM to Profit Sharing, the utility added was deemed by our community to justify the moderate additional cost to enter or exit the pool.

### iFARM

The interest bearing FARM token, iFARM, is a deposit receipt token for FARM that is auto compounding in the Profit Sharing pool. It can be obtained by selecting the "Use iFARM" box when depositing farm into the Profit Sharing pool.

 iFARM utilizes the same [vault architecture](../../how-it-works/harvest-contracts/vaults/) as Harvest's other vaults, colleting FARM from users and then depositing it in aggregate into the Profit Sharing pool. The advantages of iFARM over FARM include:

* Lower gas costs to deposit FARM into profitsharing.
* A fungible and transferrable receipt token, iFARM, allowing compounding Profit Sharing shares to be transferred between addresses without first unstaking FARM.
* Composability of the iFARM token allows compounding Profit Sharing shares to be utilized in external opportunities, such as providing liquidity for iFARM on Matic, or minting fCASH.

![](../../.gitbook/assets/ps-2.png)

{% hint style="warning" %}
Note: because there is typically some un-invested FARM in the vault, the iFARM vault has a slightly lower rate of return than FARM staked directly to profitsharing. Due to the high adoption rate of iFARM, the discrepancy is typically extremely small \(&lt;0.1% at the time of writing\).

In addition, withdraws of FARM in amounts greater than the un-invested FARM held in the vault may require more gas than withdrawing from the Profit Sharing pool directly.
{% endhint %}

## What is the Profit Sharing pool? 

Profit Sharing pool allows users to stake farmed FARM tokens to receive 30% of Harvest Finance protocol profits. The most popular strategies for use Profit Sharing pool is collecting FARM through regular farming of many assets available on Harvest Finance, or simply buying FARM token on the market to join the profit sharing pool.





Harvest Finance profits are regularly distributed to Profit Sharing pool through FARM token automatically bought on the market and distributed to the pool, users of the pool can expect to have their FARM tokens deposited to auto compound in the rate showed by the APY on the pool. 

### Why the Profit Sharing APY goes up and down, shouldn't it be 30%?

While 30% of Harvest Finance profits are regularly distributed to the Profit Sharing pool it does not actually mean the pool APY should be 30% as Harvest Finance profits are not accumulated to be distributed immediately but distributed regularly over time, there are many reasons why APY goes up and down, it may be sometimes due to governance decisions on incentives like the amount of FARM emissions directed to Profit Sharing pool, fundamental tokenomics dynamics as the 4% emission reduction every week, or even swings in price of FARM token can deviate the short term APY from the base 30%. Market volume in LP assets farmed can also have an impact in the APY movement as a high volume in a LP position generally captures more fees driving up APY, while FARM token price could not immediately moving accordingly in the short term. Other factors that can affects Profit Sharing APY are Total Value Locked in Harvest Finance and FARM token price, generally when TVL decreases we can expect the Profit Sharing pool APY to decreases and when FARM price deviates too much from it's value we can also expect a swing in the Profit Sharing APY.

## Resources

You can check how to join in the Profit Sharing pool [here](https://www.youtube.com/watch?v=VxSgvj8lmNM)  \(Credits to [Coinstruct](https://www.youtube.com/channel/UCywRgYh3qQ45savdWcY9o0A)\).  
  
You can check FARM token buybacks data, weekly profit, and FARM token PE ratio [here](https://farmdashboard.xyz/).

It is possible to check the live FARM distribution to Profit Sharing on [harvests ](https://discord.com/channels/748967094745563176/758266916095393792)Discord topic.



