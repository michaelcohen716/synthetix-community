---
id: seth-pool
title: ETH/sETH Pool
sidebar_label: ETH/sETH Pool
---

## Overview

Synthetic Ether (sETH) is a soft peg of standard ether (ETH), designed to stay as close in value as possible. In the early days, however, sETH has often traded at a discount, making it difficult for traders to move seamlessly between the collateralized and synthetic worlds without incurring high costs. 

Uniswap's constant product model forces the price of sETH lower when the demand for ETH is higher. However, the larger the ETH/sETH liquidity pool grows, the less impact any one trade has. As such, Synthetix encourages investors to add liquidity to the pool by offering SNX incentives. Synthetix hopes that the combination of these rewards and the <a href="/docs/arb-pool" class="link">Arbitrage Pool</a> incentives will bolster a strong peg.

Read more about liquidity pool staking here: <a href="https://sips.synthetix.io/sips/sip-8" class="link" target="_blank">SIP 8: sETH Uniswap Pool Staking Incentives</a>

As of February 2020, the ETH/sETH pool is the largest on Uniswap by far, owing largely to protocol incentives.

## Basic Steps
- Collect an equal combination of ETH and sETH (Uniswap expects a value-equivalent liquidity contribution)
- Go to the `Pool`/`Add Liquidity` tab on <a href="https://uniswap.exchange/add-liquidity" class="link" target="_blank">Uniswap</a>
- Populate the value fields to add your liquidity to the pool and confirm the transaction
- Then, follow the steps <a href="https://help.synthetix.io/hc/en-us/articles/360043634533" class="link" target="_blank">laid out in the blog post</a> from the team 

## Rewards Calculations
Synthetix distributes 5% of weekly inflation to liquidity providers. As of March 2020, 64,000 SNX are distributed weekly, but this figure will decline gradually as the inflation schedule progresses. The <a href="https://etherscan.io/address/0x48d7f315fedcad332f68aafa017c7c158bc54760" class="link" target="_blank">Unipool rewards contract</a> calculates rewards proportionally to time spent in pool. 

## Rewards Distributions
You'll need to actively claim your liquidity provider rewards from the contract linked above following the instructions in the team's post linked above. For the new Unipool contract, there are no time constraints on claiming rewards. They'll be available whenever you want to claim them.  
