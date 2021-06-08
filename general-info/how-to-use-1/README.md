---
description: User guides and tutorials
---

# How to use Harvest

Prior to getting started, we highly recommend that users have some understanding of how the Ethereum network functions. The following will serve as a very basic overview of topics that should be familiar to users.

#### Wallets

An Ethereum wallet allows users to interface and send initialize Ethereum transaction with a unique \(and public\) Ethereum address that holds their tokens and funds. The majority of Harvest users utilize the Metamask browser extension; however, WalletConnect may also be used to connect with mobile wallets. Users will need to be comfortable buying/selling tokens to make use of Harvest.

#### GAS

To be included and confirmed on the blockchain, a given transaction must be mined. To this end, each transaction includes a small ETH tip for the first miner that incorporates it. Because Ethereum smart contracts require variable amounts of computational complexity \(GAS\), most users interface with this tip by setting a GAS price. Transactions are mined on a first-come, first-serve basis, meaning that higher gas prices are generally mined faster; however, GAS prices fluctuate with network activity, and predictions for time to confirmation made by wallets are not always accurate. 

{% hint style="danger" %}
For safety purposes, Ethereum wallets include a `nonce` with each transactions. All transactions must be confirmed **in order**, ****so sending a new transaction with a higher gas price will **NOT** cause it to confirm more quickly, but **will** cost you additional ETH once confirmed. If you are struggling with stuck transactions feel free to ask for support in Harvest Finance [Discord server](https://discord.com/invite/gzWAG3Wx7Y).
{% endhint %}

{% hint style="info" %}
Most of the transactions on Harvest are not stateful, and can therefore be sent using relatively low GAS prices if the user is willing to wait a long time for confirmation. 
{% endhint %}



