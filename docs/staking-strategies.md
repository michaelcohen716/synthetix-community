---
id: staking-strategies
title: Strategies
sidebar_label: Strategies
---

## Liquidation risk
A key factor to keep in mind when formulating a staking strategy is the risk of liquidation. As described in <a href="https://blog.synthetix.io/liquidation-faqs/">the liquidation blog post</a> and <a href="https://sips.synthetix.io/sccp/sccp-25">this liquidation proposal</a>, your stake is at risk of liquidation if your collateral ratio (`C-RATIO`) has gone under 200%, and remained less than 500% for more than three days. You should aim to keep your `C-RATIO` well above that, and check it at least every three days. Note that these thresholds are subject to change.

## Conservative Strategy
A conservative staker doesn't mint the maximum amount of sUSD, but instead targets an initial `C-RATIO` of 800%-900%. If the value of SNX increases and their ratio moves significantly above 900%, the conservative staker might consider minting more sUSD to restore the target ratio range. This staker will use sUSD minted to mirror the global synth portfolio on <a href="https://dashboard.synthetix.io/" class="link" target="_blank">Synthetix Dashboard</a>.

## Neutral Strategy
A neutral staker targets an initial `C-RATIO` of 725%-775%. If the value of SNX increases and their ratio moves well above 725%, the neutral staker would consider minting more sUSD to restore a ratio within the target range. This staker might exchange sUSD for ETH, loan out sUSD, or trade for other synthetics, but more likely they would try to align with the global synth portfolio.


## Aggressive Strategy
An aggresive staker mints the maximum amount of sUSD and continues to mint as the SNX value increases. If the SNX value decreases, the aggressive staker might need to hold a reserve of SNX or ETH to acquire enough SNX to restore the ratio in order to claim rewards. Alternatively, they may <a href="/docs/transferring-snx#burning-susd" class="link">burn sUSD</a> to bring their ratio back above 600%.) The staker would use their minted sUSD in whichever way most reflects their market view. 

## Hyper-Aggressive Strategy
A hyper-aggressive staker mints the maximum sUSD and uses that sUSD to buy more SNX, then uses the new SNX to mint more sUSD to buy more SNX. This is super risky and may not end well.
