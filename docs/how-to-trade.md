---
id: trading-como
title: Como Tradear Trading Sintéticos
sidebar_label: Como Tradear Sintéticos
---

## Accessing the Ecosystem
There are three easy ways to acquire the assets needed to trade on <a href="https://synthetix.exchange/" target="_blank" class="link">Synthetix Exchange</a>:
- <a href="/docs/staking-snx-overview" class="link">Stake SNX</a> and mint sUSD to trade
- Use Uniswap to exchange ETH for sETH to trade on Exchange
- Use the utility on the left panel of the Exchange interface to exchange ETH for sUSD

## Executing a Trade
The interface will populate with your balances in each synthetic asset. As of November 2019, there are ~25 supported assets, with many more planned. Some are protocol level long assets like sETH and sBTC, paired with an inverse short asset. Some are Ethereum tokens - again, paired with an inverse short version - and some are global fiat currencies. The team has also introduced synthetic baskets of assets, with short/long pairs of a centralized exchange token basket available and a decentralized finance basket available soon.

Traders can execute a transaction by selecting an input asset, an output asset and an amount. The trading fee is 0.3% of the transaction value.

> The fee has been 0.5% at times recently, to reduce the profitability of front-running bots

For trades exchanging a long asset for an inverse asset (e.g. sETH for iBTC), the fee is doubled. Crucially, there is no slippage. The spot price for 1 sETH is the same as for 100 sETH. 

The Exchange interface allows the trader to choose from a range of transaction speeds. Beyond speed of transaction confirmation, selecting a slower or faster gas value won't affect the trade itself. However, if the network is highly congested, the trade may fail if the token is no longer available at the same price. 
