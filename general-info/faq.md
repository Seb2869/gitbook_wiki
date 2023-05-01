# FAQ

## Common Questions <a href="#common-questions" id="common-questions"></a>

* Should I interact with the contract directly? **NO**, please use the website and ask for help in #support channel in Harvest Discord.
* Is Harvest audited? [Yes](security/audites.md)
* Who is the Harvest team? **The Harvest Finance launch team is anonymous**
* I deposited into a Pool for a few hours but still have no yield. **Why?** While FARM emissions start accruing immediately after depositing, yields from farmed tokens come after a successful [doHardWork()](../how-it-works/dohardwork.md). Profitability analysis is done on when to run the doHardWork() function. Please take a look at [Vault info](../how-it-works/harvest-contracts/vaults/) and [APY calculations](how-to-use-1/how-to-understand-how-much-you-earn/apy-calculation.md) for more context.
* How is APY / APR calculated for the Pools? [**APY formulas**](how-to-use-1/how-to-understand-how-much-you-earn/apy-calculation.md) **and** [**Interest rate guid**](how-to-use-1/how-to-understand-how-much-you-earn/interest-rate-guide.md)
* How many FARM tokens are there? [**FARM tokens are capped at 690,420 tokens minted over a 4-year period**](https://farm.chainwiki.dev/en/supply)
* Are there fAssets shareprice charts? Use [farmdashboard.xyz](https://farmdashboard.xyz/)
* Where can I trade FARM tokens? [Where trade FARM](how-to-use-1/where-trade-farm-bfarm.md)
* How do I turn tokens into Harvest `fTokens` that earn yield farming revenue? [**on the Harvest front page**](https://harvest.finance/)
* How do I turn`fTokens` tokens back into regular tokens? [**withdrawal instructions**](how-to-use-1/how-to-deposit-withdraw.md)
* Do FARM tokens get yield farming revenue just by holding them? **FARM must be deposited in** [**Profit Sharing**](what-do-we-do/profit-sharing-pool-ps.md) to earn yield farming revenue.
* How much yield farming revenue is shared with Profit Sharing stakers? **30% of yield farming revenue on ETH and 8% on BSC.** [**PS Pool** ](what-do-we-do/profit-sharing-pool-ps.md)
* What happens to the other 70% of yield farming revenue? **It is paid out to users that deposit assets to Harvest for farming**. Over time, holders of Harvest farming fTokens will receive more of the underlying tokens when they withdraw.
* What is iFARM? **iFARM is the interest bearing FARM token, it works as FARM staked in the profit share and it's main advantages is a lower gas cost, transferability and possible future new utilities like lending collateralization as an exemple.**
* Why does the Profitshare APY go up and down? **There are many reasons why APY goes up and down, it may be sometimes due to governance decisions on incentives like the amount of emissions directed to profit share, fundamental tokenomics dynamics as the 4% emission reduction every week, or even swings in price of FARM token can deviate the short term APY from the base 30%. Market volume in LP assets farmed can also have an impact in the APY movement as a high volume generally in a LP position captures more fees driving up the APY.**
* The 30% fee from profit share is charged from the APY in farms shown in the front page? **No. The APY shown in the front page was already charged by the 30% Profit Share fee, they are the final APY.**

## Technical Stuff <a href="#technical-stuff" id="technical-stuff"></a>

* Is the code open source? [**contracts are**](https://github.com/harvest-finance/harvest)**; frontend UI is not currently** (to slow down clones)
* Why is the fee to deposit and withdraw stablecoins so high? In some cases, **withdrawing must remove stablecoins from yield farming strategies**; come back later for lower fees
* I want to see the yield farming revenue paid to FARM Profit Share. [Example of doHardWork](https://etherscan.io/tx/0x9b68d4559be71702b9b8084d2b410d241b9542a956f27aa88fc62b4e12fdebdf)
* I want to audit the funds that Harvest is using for yield farming. You can find all info on the [farmdashboard.xyz](https://farmdashboard.xyz/)
* How can I tell that the Harvest fStablecoins are changing in value due to yield farming? Look at the [**fDAI**](https://etherscan.io/address/0xe85c8581e60d7cd32bbfd86303d2a4fa6a951dac#readContract)**,** [**fUSDC**](https://etherscan.io/address/0xc3f7ffb5d5869b3ade9448d094d81b0521e8326f#readContract)**, or** [**fUSDT**](https://etherscan.io/address/0xc7ee21406bb581e741fbb8b21f213188433d9f2f#readContract) **contracts.** The value that converts from fTokens to tokens is `getPricePerFullShare`. This has the same number of decimals as the underlying stablecoin and will increase over time if yield farming is profitable.
* Are there timelocks? **Yes, 12 hours.** [**Timelocks**](../how-it-works/harvest-contracts/vaults/timelocks.md)
* How can I help? **Glad you asked.** [**Join Harvest on Discord**](https://discord.gg/R5SeTVR)**, Become a** [**Builder**](../builders.md)
