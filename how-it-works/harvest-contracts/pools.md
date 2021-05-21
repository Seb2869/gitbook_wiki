# Pools

A Reward Pool, or Staking Contract is an ethereum scaling solution for providing rewards to users over time.

It is in Harvest's interest to attract new users to its platform to provide additional deposits for its investment strategies and liquidity to the FARM token so that users can buy and sell FARM. To that end FARM emissions are provided as incentives, which are distributed to users pro rata via reward pools.

Users provide their proof of investment in the form of an `fASSET` \(or `UNI-V2` FARM:ETH LP token in the case of liquidity providers\). The user's address is then credited with FARM for each second that the proof of investment remains in the reward pool.  
The rewards pool offers two functions:

* Claim: The contract sends the user any accumulated FARM rewards, but retains the staked `fASSET` to continue accumulating rewards.
* Unstake and Claim: Calls the `exit()` function of the contract, which returns the staked `fASSET` to the user's address in addition to any accumulated FARM rewards.

Harvest generally displays the reward rate of the staking contract in the form of an "APY." This represents the instantaneous per-second reward rate per dollar value of the staked `fASSET`. The reward rate is determined as follows:

1. At the start of each weak, "emissions" of FARM are sent as a lump sum to each reward pool contract by the devs. These numbers are published in the weekly Harvest medium post.
2. The rewards are 'notified' by the devs, indicating that they should begin paying out.
3. For every second that passes, the emitted amount/604800 \(number of seconds in a week\) are distributed pro rata to every address with staked fassets.

Please note that the greater the participation in a rewards pool, the lower the reward payed to each participant per second \(and therefore APY\) becomes.

