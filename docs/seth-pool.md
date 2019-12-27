---
id: seth-pool
title: ETH/sETH Pool
sidebar_label: ETH/sETH Pool
---

## Overview

Synthetic Ether (sETH) is a soft peg of standard ether (ETH), designed to stay as close in value as possible. In the early days, however, sETH has often traded at a discount, making it difficult for traders to move seamlessly between the collateralized and synthetic worlds without incurring high costs. 

Uniswap's constant product model forces the price of sETH lower when the demand for ETH is higher. However, the larger the ETH/sETH liquidity pool grows, the less impact any one trade has. As such, Synthetix encourages investors to add liquidity to the pool by offering SNX incentives. Synthetix hopes that the combination of these rewards and the <a href="/docs/arb-pool" class="link">Arbitrage Pool</a> incentives will bolster a strong peg.

Read more about liquidity pool staking here: <a href="https://sips.synthetix.io/sips/sip-8" class="link" target="_blank">SIP 8: sETH Uniswap Pool Staking Incentives</a>

As of November 2019, the ETH/sETH pool is the largest on Uniswap by far, owing largely to protocol incentives.

## Basic Steps
- Collect at least 1 ETH and 1 sETH token
- Go to the `Pool`/`Add Liquidity` tab on <a href="https://uniswap.exchange/add-liquidity" class="link" target="_blank">Uniswap</a>
- Populate the value fields to add your liquidity to the pool and confirm the transaction
- Ensure that you've collected at least 1 <a href="https://etherscan.io/token/0xe9cf7887b93150d4f2da7dfc6d502b216438f244" target="_blank" class="link">liquidity token</a> from the pool. You'll be ineligible for rewards if you have fewer

## Rewards Calculations
Synthetix distributes 5% of weekly inflation to liquidity providers. As of November 2019, 72,000 SNX are distributed weekly, but this figure will decline gradually as the inflation schedule progresses. The team takes a snapshot of active stakers each Wednesday at roughly 09:00 UTC to determine pro rata allocations. 

<a href="https://docs.google.com/spreadsheets/d/14qQKeprY3IQBT2p-jDrnKMBKNpOh0-rRDZSlBwBYXV0/edit#gid=459184262" class="link" target="_blank">This spreadsheet</a> has week-to-week reward calculations

## Rewards Distributions

Unlike with staking rewards, you don't need to actively claim liquidity pool rewards. They will be sent directly to your address. But to ensure you're not disqualified from receiving rewards, you'll need to:
- have at least one liquidity token
- have not removed any liquidity during the Wednesday-to-Wednesday period
- have been providing liquidity to the pool for the entire week period

Because validating and distributing these rewards is still a manual process, the distributions are running on a roughly one week lag. For the week ending this Wednesday, you may not be paid until the following Wednesday or Thursday.

There are efforts underway to <a href="https://github.com/k06a/Unipool/blob/master/contracts/Unipool.sol" class="link" target="_blank">programmatically calculate and distribute rewards</a>.