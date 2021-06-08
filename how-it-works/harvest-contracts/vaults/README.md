# Vaults

A vault is an Ethereum scaling solution that allows users to safely deposit and withdraw funds from a pool of investable assets.

![](https://farm.chainwiki.dev/vault_draft.png)

When a user deposits funds, they are issued a share of the vault, represented by an `fASSET`. These user's funds are then made available for investment according to a pre-defined "strategy" specified by the Harvest devs. Whenever an investment strategy generates revenue \(or losses\), the total amount of assets in the Vault is updated, however the number of existing `fASSET` shares does not change. As a result, the value of each `fASSET` share increases with every successful harvest. When a user withdraws `fASSET` shares from the vault, the `fASSET` is burned and the user receives funds proportional to the growth of the investment since their deposit.

![](https://farm.chainwiki.dev/vault_draft2.png)

Most of Harvest's strategies function by investing the underlying assets into incentivized liquidity pools for various other protocols. Harvest automatically compounds its interest by selling the incentived rewards into more of the underlying vault asset and reinvesting it. While harvest may show that your deposit is "farming" some particular token, you will only receive the token you deposited, unless otherwise specified.

User funds are protected in vaults by a number of mechanism:

1. The owners of the vault can only move the underlying funds in and out of the pre-defined investment strategy.
2. `fASSET`shares can only be minted by depositing funds into the vault, and are destroyed when the user withdraws funds.
3. The investment strategy is protected from changes by a '[timelock](https://harvest-finance.gitbook.io/harvest-finance/how-it-works/harvest-contracts/vaults/timelocks).' 

Harvest Vaults do not track the wallet addresses of depositors. Instead, `fASSET` shares are represented by fungible ERC-20 tokens that can be transferred between accounts and traded on secondary markets. Users that trade away or lose their `fASSET` shares will not have access to their deposited funds.

Because Ethereum gas usage is defined by the number of contracts interacted with and the complexity of the interactions, depositing tokens through the Vault smart contract and minting new `fASSET` shares requires significantly more gas than than the token trading that most Ethereum users may be used to. Users should take care to monitor gas expenses, as they may reduce or even overwhelm the profitability of smaller scale investments \(&lt;$1000\), especially when network activity is high.

Harvest provides additional incentives for users to deposit funds in the form of `FARM` tokens. These rewards are distributed to users who prove ownership of deposits by staking their `fASSETs` in reward pool contracts. It is important to note that before a user can withdraw funds, they must first retrieve their `fASSET` from a reward pool staking contract.

