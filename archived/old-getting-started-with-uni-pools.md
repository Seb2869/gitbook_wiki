# \(Old\) Getting Started with UNI Pools

> **It's an old tutorial and some information out of date**

## Intro ![&#x1F33D;](https://farm.chainwiki.dev/_assets/svg/twemoji/1f33d.svg) <a id="intro"></a>

Welcome back city slicker! Now that you roughed up your hands in the [first tutorial](farm-with-usdc.md), let's start chasing some of that crazy APY in some other pools. How about the Uniswap Pool? That APY is way up there!

Sounds too good to be true, you say? Good point. You need to understand the risk if Impermanent Loss by playing in this pool.

> If you don't understand IL, I highly suggest you stop right here and do a little homework. Personally, I had to watch [this video](https://www.youtube.com/watch?v=8XJ1MSTEuU0) and read [this blog](https://blog.bancor.network/beginners-guide-to-getting-rekt-by-impermanent-loss-7c9510cb2f22) a good 3 times or so for it to finally sink in.  
> tl;dr this [Tweet](https://twitter.com/Fiskantes/status/1314524664484503555) from [@Fiskantes](https://twitter.com/Fiskantes) pretty much sums it up...  
> ![getting\_started\_uni\_good\_lp.png](https://farm.chainwiki.dev/getting_started_images/getting_started_uni_good_lp.png) ![getting\_started\_uni\_bad\_lp.png](https://farm.chainwiki.dev/getting_started_images/getting_started_uni_bad_lp.png)

So you do want to live on the edge! Okay! Let's get going!

## Here's What We're Going to Do ![&#x1F69C;](https://farm.chainwiki.dev/_assets/svg/twemoji/1f69c.svg) <a id="heres-what-were-going-to-do"></a>

To participate in the Uniswap LP Farm, we will need to supply USDC-FARM liquidity to Uniswap's Liquidity Pool. Then use Uniswap LP tokens minted from that transaction to deposit into the Farm.

1. Get USDC \(not sure how? Go to the previous tutorial\)
2. Swap half of our USDC for FARM
3. Deposit USDC and FARM into Uniswap's Liquidity Pool. Receive UNI\_LP tokens
4. Deposit UNI\_LP Token into Farm
5. Profit! ![&#x1F35E;](https://farm.chainwiki.dev/_assets/svg/twemoji/1f35e.svg)

> These steps total 6 transactions on the Ethereum blockchain. Be wary of gas prices before you start. Make sure you have enough ETH in your Wallet. Gas was at ~50 Gwei at time of doing this tutorial.

## Get USDC ![&#x1F349;](https://farm.chainwiki.dev/_assets/svg/twemoji/1f349.svg) <a id="get-usdc"></a>

Alright, you should already know how to do this if you followed the [first tutorial](farm-with-usdc.md).  
In the next step, we will be exchaning half \(by value\) of our USDC for FARM. So make sure you have enough USDC to split.

## Buy FARM ![&#x1F353;](https://farm.chainwiki.dev/_assets/svg/twemoji/1f353.svg) <a id="buy-farm"></a>

Now, with our USDC, we are going to swap half of it for FARM

> This will happen in two steps. An Approval and a Swap step. Both will charge gas!

* Click Buy FARM on the top of the [harvest.finance](https://harvest.finance/) page. It will take you to Uniswap to Swap USDC for FARM. ![getting\_started\_uni\_buy\_farm.png](https://farm.chainwiki.dev/getting_started_uni_buy_farm.png)
* OMG! SCARY WARNING ![&#x1F631;](https://farm.chainwiki.dev/_assets/svg/twemoji/1f631.svg) ![getting\_started\_uni\_uni\_warning.png](https://farm.chainwiki.dev/getting_started_uni_uni_warning.png)

> The warning says exactly what it means. It's up to you to make sure the addresses you are using are correct. You might want to click on those View on Etherscan links and verify them against [Harvest's Github page](https://github.com/harvest-finance/harvest).

* All set? Okay! Take half of our USDC and Swap it for FARM! in this case, we have 1500 USDC. So we will use 750 for the SWAP.! ![getting\_started\_uni\_swap\_usdc\_farm\_approve.png](https://farm.chainwiki.dev/getting_started_uni_swap_usdc_farm_approve.png)
* Once the Approval goes through, we will now do the Swap! ![getting\_started\_uni\_swap\_usdc\_farm\_swap.png](https://farm.chainwiki.dev/getting_started_uni_swap_usdc_farm_swap.png)
* Hooray! We now have USDC and FARM in our Wallet to add to the Liquidity Pool ![getting\_started\_uni\_metamask\_farm\_usdc.png](https://farm.chainwiki.dev/getting_started_uni_metamask_farm_usdc.png) _I know, I know. You are wondering where I accumulated all that DAI and FNT. That's none of your business!_

## Add FARM and USDC to UNI LP ![&#x1F34E;](https://farm.chainwiki.dev/_assets/svg/twemoji/1f34e.svg) <a id="add-farm-and-usdc-to-uni-lp"></a>

With the USDC and FARM in our Wallet, we are going to add it to Uniswaps USDC-FARM Liquidity Pool.

> This will also require two transactions: Approve and Supply

* Click Earn on the top of Harvest.Finance. Then select the Uniswap Farm
* ![getting\_started\_uni\_select\_uni\_farm.png](https://farm.chainwiki.dev/getting_started_uni_select_uni_farm.png)
* Select UNI-V2. This will take you to Uniswap's USDC-FARM Pair page ![getting\_started\_uni\_acquire\_uni\_lp\_tokens.png](https://farm.chainwiki.dev/getting_started_images/getting_started_uni_acquire_uni_lp_tokens.png)
* At the top right of the page, select Add Liquidity ![getting\_started\_uni\_add\_liquidity.png](https://farm.chainwiki.dev/getting_started_images/getting_started_uni_add_liquidity.png)
* Select Max FARM \(or USDC\)! Then click Approve ![getting\_started\_uni\_approve\_liquidity.png](https://farm.chainwiki.dev/getting_started_images/getting_started_uni_approve_liquidity.png)
* Once Approve transaction goes through, Click Supply ![getting\_started\_uni\_supply\_liquidity.png](https://farm.chainwiki.dev/getting_started_images/getting_started_uni_supply_liquidity.png)
* After this transaction, Uniswap will show your positions in the Pool ![getting\_started\_uni\_lp\_positions.png](https://farm.chainwiki.dev/getting_started_images/getting_started_uni_lp_positions.png)
* We received 0.0000657 UNI\_LP-V2 tokens that we will use in the next step
* Congrats! you are now a Liquidity Provider for Uniswaps USDC-FARM Liquidity Pool! You are now earning fees off user's exchange transactions from this pool. Of course, now you are also at risk of Impermanent Loss ![&#x1F631;](https://farm.chainwiki.dev/_assets/svg/twemoji/1f631.svg) ![&#x1F631;](https://farm.chainwiki.dev/_assets/svg/twemoji/1f631.svg) ![&#x1F631;](https://farm.chainwiki.dev/_assets/svg/twemoji/1f631.svg)

## Deposit Tokens in to UNI LP Farm ![&#x1F331;](https://farm.chainwiki.dev/_assets/svg/twemoji/1f331.svg) <a id="deposit-tokens-in-to-uni-lp-farm"></a>

> This will also require two transactions: Approve and Stake

Time to put our UNI\_LP tokens into the Farm and earn some of that high yield FARM!

* Back on the Harvest's Uniswap Farm page, we now have the ability to Stake. Select Max, then select Stake ![getting\_started\_uni\_stake\_uni\_lp.png](https://farm.chainwiki.dev/getting_started_images/getting_started_uni_stake_uni_lp.png)
* In our Wallet, we will do 2 transactions: Approve and Stake. I'm tired of taking screen shots; you're on your own for that
* All done! We are staked in the Farm, earning that sweet APY! ![getting\_started\_uni\_stake\_complete.png](https://farm.chainwiki.dev/getting_started_images/getting_started_uni_stake_complete.png)

> I went to Uniswap and don't see my posiitons!! When you add your UNI\_LP tokens to Farm, you temporarily stake your LP tokens into Harvest, and Harvest use it to farm and sell crops to grow the amount of your LP. The value of your LP still grows with each trade on the Uniswap pool. So you get to enjoy Harvest's automated golden crops on top of Unicorn yields.

## Earn FARM! ![&#x1F35E;](https://farm.chainwiki.dev/_assets/svg/twemoji/1f35e.svg) <a id="earn-farm"></a>

Farming is good honest work. You did great my fellow farmhand. Let's now watch the fruits of our labor!

* Navigate to the [Harvest Finance Dashbaord](https://harvestfi.github.io/dashboard/) ![getting\_started\_uni\_harvest\_dashboard3.png](https://farm.chainwiki.dev/getting_started_images/getting_started_uni_harvest_dashboard3.png)
* We now see ouf FARM\_USDC\_LP there and the staked balance of UNI\_LP we added.
* Assets at the bottom will include the Underlying USDC and FARM that we added to the Liquidity Pool.

