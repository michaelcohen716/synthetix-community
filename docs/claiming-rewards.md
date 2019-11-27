---
id: reclamando-ganancias
title: Reclamando Ganancias
sidebar_label: Reclamando Ganancias
---

## Pasos Básicos
- Las ganancias son calculadas y habilitadas una vez cada semana, específicamente los Miércoles.
- Use <a class="link" target="_blank" href="https://beta.mintr.synthetix.io/">Mintr</a> para navegar a la sección de Reclamación (`Claim`).
- Asegúrese de que su ratio de colateralización (C-Ratio) es suficiente para reclamar: es requerido un 750%, pero si está en un rango del 1% (sobre 742.5%, por ejemplo), no tendrá problemas para realizar su petición. En caso contrario, usted tendrá que <a href="/docs/buying-snx" class="link"> comprar más SNX</a> o <a href="/docs/transferring-snx#burning-susd" class="link">quemar sUSD</a> para restablecer su `C-RATIO`.
- Presione `Claim Now` para cobrar su ganancia semanal, tanto en sUSD como en SNX.
- Usted debe realizar al menos una reclamación cada dos semanas. De no hacerlo, sus ganancias serán devueltas al fondo de recompensas común al término de dicho plazo.
- Los SNX reclamados como ganancia son mantenidos en custodia (`escrowed`) por un año. Usted no podrá transferirlos o venderlos durante ese periódo.


## Managing Debt
Your `C-RATIO` can change without any direct action by you. There's a <a href="https://help.synthetix.io/hc/en-us/articles/360023174973-Why-does-my-total-sUSD-debt-fluctuate-over-time-" target="_blank" class="link">detailed explanation here</a> on why global debt fluctuates over time. In simple terms, the global debt - and your pro rata slice of it - will increase if traders on Synthetix Exchange are profitable and decrease if they are unprofitable.

As of November 2019, the vast majority of traders on Synthetix are long `sETH` and `sBTC`, synthetic ether and bitcoin. There's a section called `Synths Distribution` on the <a href="https://dashboard.synthetix.io/" class="link" target="_blank">Synthetix Dashboard</a> with up-to-date stats on positioning. 

A common strategy to keep `C-RATIO` fairly stable is to use the sUSD you've minted to mirror the global positioning of traders. Your debt will increase if the portfolio does well, but your synth value will increase in constant terms, protecting your `C-RATIO`.

If a staker mints sUSD and doesn't trade it, they are effectively short the global portfolio, because they're exposed to an increase in global debt without a potential increase in synth holdings. There's nothing wrong with this market positioning, but some beginner stakers don't realize that they're exposed to the global portfolio.

<a href="https://www.delphidigital.io/research" target="_blank" class="link">Delphi Research</a> has a series of detailed examples on the system's debt mechanics in their report on SNX (behind paywall). See one below:

<img src="assets/debt-example.png" width="50%">


## How are rewards calculated?
There are two components to rewards: sUSD and SNX.

When a trader transacts on Synthetix Exchange, they pay a 0.3% fee. Those fees are distributed pro rata, to all stakers.

The more sUSD you've minted, the higher proportion of fees you'll receive. 

Global SNX rewards are determined by the SNX inflation schedule. As of November 2019, 90% of weekly inflation is allocated toward staking rewards. More on Synthetix's <a class="link" target="_blank" href="https://blog.synthetix.io/synthetix-monetary-policy-changes/">monetary policy here</a>. 

If you are below the target `C-RATIO`, you will not be penalized. You just won't be able to claim your rewards.

Your proportion of global debt is calculated based on a `snapshot` of the network taken every Wednesday at roughly 09:00 UTC.

## Calculating Returns
Returns are a function of Synthetix Exchange volume, the current inflation schedule, and an individual staker's proportion of global minted debt. <a href="https://www.stakingrewards.com/asset/synthetix-network-token" class="link" target="_blank">Staking Rewards</a> provides an approximation of expected SNX returns, but it may not include the value of sUSD returns.


