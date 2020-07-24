---
id: other
title: Other FAQs
sidebar_label: Other FAQs
---

## Where do Synth price feeds come from? 

Synthetix has partnered with Chainlink, whose network of independent node operators supply [price feeds](https://feeds.chain.link/) for our fiat currencies and commodities. 
We will be furthering the integration with Chainlink in the future to cover the rest of the Synths. 

Price feeds not yet supplied by Chainlink are supplied by a centralised oracle that will be deprecated when the transition is complete. 

[Here](https://etherscan.io/address/0xac1ed4fabbd5204e02950d68b6fc8c446ac95362) is the Synthetix oracle address. 

## Why is it important to incentivise people to create a Synth liquidity pool? 

There is currently an sUSD liquidity pool on [Curve](https://beta.curve.fi/) where people can use other stablecoins to purchase sUSD, and vice versa. 

The Curve pool is a decentralized way to provide on/off ramps to the Synth system, so newcomers can start trading easily and exit the system easily. Changes in the exchange rate are bad for liquidity providers (i.e. [impermanent loss](https://tokentuesdays.substack.com/p/eliminating-impermanent-loss)). 
Since the sUSD/stablecoin ratio should be pretty much constant, that pool is ideal for liquidity providers: there is no impermanent loss so the liquidity providers should end up getting all of the exchange fees. To make it even more enticing for LPs, some of the SNX inflationary reward has been diverted to them. The result is a deep liquidity pool, which is good for the Synth ecosystem. 
Before this liquidity pool, the main way to get in and out of trading on Synthetix.Exchange (other than by minting) was to use thin markets on centralized exchanges.

## Why aren't my SNX tokens showing up in Etherscan (or another platform)?

There are several reasons why they might not be showing up. The most common reason is that you were affected by the proxy contract cutover on [May 10](https://blog.synthetix.io/proxy-contract-cutover-on-may-10/). This can look like [this](https://ibb.co/0DWzZQN). 
If you want them to show up on that platform, you'll need to 'emit an event' with your SNX by interacting them in some way. The simplest way is by sending yourself (i.e. to your own wallet) a transfer for 0 SNX. using this token address: [0xC011a73ee8576Fb46F5E1c5751cA3B9Fe0af2a6F](https://etherscan.io/token/0xc011a73ee8576fb46f5e1c5751ca3b9fe0af2a6f). Please note you'll need some ETH in your wallet to pay for gas. 

One other reason is that your SNX is still escrowed from the Havven token sale — they can be vested through [Mintr](https://mintr.synthetix.io) in the ESCROW tab by clicking on the 'View Token Sale Escrow' button.

## Why are my transactions still pending? 

[Here's a useful guide](https://ethgasstation.info/blog/stuck-transaction-guide/)

## Why are Synthetix transactions so expensive? 

Transactions cost a certain amount proportional to how much processing power is required for Ethereum miners to process it. The Synthetix system and tokens are more complex than the majority of other Ethereum projects, so its transactions—including simple token transfers—require more gas to be completed. 

If you are used to tokens that are far cheaper to interact with or transfer, that is because they can do far less than the tokens in the Synthetix system. Unfortunately the tradeoff for having a token that can do many things is that it can cost more. The best way to get around this is to try to pay as low GWEI as possible. For more info on how gas works on Ethereum, see [this article](https://blockgeeks.com/guides/ethereum-gas/). 
