---
id: arb-pool
title: Poolde Arbitraje
sidebar_label: Pool de Arbitraje
---

## Visión General

Along with the <a href="/docs/seth-pool" class="link">ETH/sETH liquidity pool incentives</a>, the Arbitrage Contract is designed to bolster the ETH/sETH soft peg, ensuring that traders have a clean, cost-effective on-ramp and off-ramp between the collateralized and synthetic worlds. 

The contract is external to the Uniswap liquidity pool, but routes all transactions through it. When the ratio of sETH to ETH falls below 0.99, users can send ETH to the contract which will first convert the ETH to sETH and then convert the sETH to SNX. Uniswap's constant product model forces the price of sETH higher when the relative demand is higher, so this multi-step transaction serves to bolster the peg.

Read more about the arbitrage contract here: <a href="https://blog.synthetix.io/our-new-seth-snx-arb-contract-is-now-live/" class="link" target="_blank">Our new ETH-SNX arb contract is now live!</a>

## Basic Steps

- Navigate to the <a href="https://etherscan.io/dapp/0xa6b5e74466edc95d0b6e65c5cbfca0a676d893a4#writeContract" class="link" target="_blank">Etherscan Dapp</a>

- Connect to your Web3 provider (top right corner)
- Click on the contract address (top left corner) and ensure that the contract still has an SNX balance. It's refilled every week but sometimes the reserve is spent. Return to the Dapp
- Click `arbSynthRate` (#13) and enter the ETH amount you want to send
- Confirm transaction

## Incentive Calculations
Synthetix allocates 5% of weekly inflation to the arbitrage contract. As of November 2019, 72,000 SNX are distributed weekly, but this figure will decline gradually as the inflation schedule progresses. Once the contract is emptied, it won't be refilled until the new week. 

