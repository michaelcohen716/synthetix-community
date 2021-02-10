---
id: how-to-trade
title: How to Trade
sidebar_label: How to Trade
---

## Accessing the Ecosystem
There are four ways to acquire the assets needed to trade on <a href="https://synthetix.exchange/" target="_blank" class="link">Synthetix Exchange</a>:
- <a href="/docs/staking-snx-overview" class="link">Stake SNX</a> and mint sUSD to trade
- Use Uniswap or DEX.AG to exchange ETH for sETH or sUSD to trade on Exchange
- Use Ether Collateral to <a href="https://synthetix.exchange/loans" class="link" target="_blank">take out a sETH loan</a> on Synthetix Exchange

## Executing a Trade
Choose a trading pair on the assets panel and enter your order size. As of April 2020 there are ~30 supported assets, with many more planned. Types of assets are:
* protocol level long assets like sETH and sBTC, paired with an inverse short asset
* Ethereum tokens - again, paired with an inverse short version
* global fiat currencies
* global equity indices
* synthetic baskets of assets, with short/long pairs (ex: centralized exchange token basket and a decentralized finance basket, now available)


Traders can execute a transaction by selecting an input asset, an output asset and an amount. The trading fee is 0.3% of the transaction value.

For trades exchanging a long asset for an inverse asset (e.g. sETH for iBTC), the fee is doubled. Crucially, there is no slippage. The spot price for 1 sETH is the same as for 100 sETH. 

The Exchange interface allows the trader to choose from a range of transaction speeds. Beyond speed of transaction confirmation, selecting a slower or faster gas value won't affect the trade itself. However, if the network is highly congested, the trade may fail if the token is no longer available at the same price.

As of the end of 2020, Synthetix has also supported shorting syntehtic assets at the contract level. In Feb 2020, <a href="https://synthetix.surge.sh/" target="_blank" class="link">a new interface</a> was implemented to help people take out a simple short. Before using this interface, be sure to read the important details about this new feature in the <a href="https://blog.synthetix.io/how-to-short-using-synthetix/" target="_blank" class="link">blog post</a> that announced it.
