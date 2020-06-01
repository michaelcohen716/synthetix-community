---
id: transferring
title: Transferring SNX or Synths
sidebar_label: Transferring SNX or Synths
---

There are some limitations to transferring the SNX tokens in your wallet. You can't transfer:
- staked tokens: the SNX that collateralize your debt up to 800%
- escrowed tokens: SNX rewards remain locked under escrow for a year after distribution

## Burning sUSD

To unlock staked tokens, press `Burn` on <a href="https://mintr.synthetix.io/" class="link" target="_blank">Mintr</a>. Press `View transferable SNX`. Here you'll be able to gauge how much SNX you can unlock for burning a given amount of sUSD. You'll need to burn enough sUSD to unlock *at least* the number of escrowed rewards tokens you have, before you'll be able to access transferable SNX. 

## Fee Reclamation

Additionally, the team has implemented a trading solution called Fee Reclamation to prevent frontrunners from taking advantage of latent price oracles. The consequence is that you may not be able to transfer or transact with a synth for several minutes following your recent transaction as the oracle confirms its most recent price. 