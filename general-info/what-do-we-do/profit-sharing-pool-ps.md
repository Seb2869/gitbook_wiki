# Profit Sharing and iFARM

A key innovation of the `$FARM` token is that it entitles holders to a performance fee \(**currently 30% ETH and 8% BSC**\) taken from Harvest's yield farming strategies. While each strategy may farm different assets, the performance fee is used to buy `$FARM` on the open market, which is then distributed to those who stake `$FARM` in the Profit Sharing pool. The price of `$FARM` is subject to consistent buy pressure as a result.

### Auto Compounding

In order to rectify the observation that the FARM reward token given to our users needed to be regularly be claimed and restaked in Profit Sharing, we added an auto compounding function to the Profit Sharing pool. Whenever _any_ user deposits or withdraws funds from the Profit  Sharing pool, the rewards for _all users_ are automatically collected and restaked to improve their returns and save long term stakers gas. While this increased the cost associated with staking FARM to Profit Sharing, the utility added was deemed by our community to justify the moderate additional cost to enter or exit the pool.

### iFARM

To further alleviate the gas costs associated with staking assets directly to the auto compounding Profit Sharing pool, we released the iFARM vault. Utilizing the same structure as the rest of our vaults, iFARM collects FARM from users and then deposits it in aggregate to the existing Profit Sharing pool. Upon deposit, users receive a fully fungible iFARM token, representing their share of the vault. As a result, iFARM can be staked for additional rewards or traded in secondary markets as a interest-bearing form of FARM.

{% hint style="warning" %}
Note: because there is typically some un-invested FARM in the vault, the iFARM vault has a slightly lower rate of return than FARM staked directly to profitsharing. Due to the high adoption rate of iFARM, the discrepancy is typically extremely small \(&lt;0.1% at the time of writing\).
{% endhint %}

