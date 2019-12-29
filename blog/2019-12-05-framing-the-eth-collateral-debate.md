---
title: Framing the ETH Collateral Debate
---
<div class="author">
<a class="link" href="https://twitter.com/mjayceee" target="_blank">@mjayceee</a>
</div>

## Background
<p>
Since the launch of Synthetix Exchange, the SNX token has been the system's sole source of collateral. Investors stake their SNX to mint liquidity &#8722; in the form of sUSD &#8722; for the network, and traders exchange that sUSD for synthetic assets. The combination of sUSD and synthetics outstanding represent the value of all assets in the system.
</p>
On the one hand, building Synthetix around a single core asset makes for simpler mechanics and a cleaner investment narrative. And because there’s a direct correlation between SNX market cap and synths outstanding, an SNX collateral model strengthens the relationship between the price of the token and the success of the project. 

On the other hand, supporting only SNX as collateral is highly limiting. SNX is less liquid and more easily destabilized than ETH, so the community has landed on a 750% minimum collateralization ratio. This is substantially higher than the 150% standard for ETH-collateralized DeFi protocols. Although the C-Ratio could change in the future, this disparity is a major challenge for two reasons. 

<!--truncate-->

First, at a recent SNX market cap of about $225 million, the maximum total liquidity for the network was $30 million. Traders on other exchanges routinely transact in values higher than the entire liquidity of Synthetix. Under the current model, scaling the platform is no guarantee. 

Second, a 750% C-Ratio suggests a maximum leverage of only ~13% (100% / 750%). For the few stakers that stake in order to trade, this leverage is unremarkable compared to competitor exchanges. 

With these reasons in mind, there’s clear momentum in the community to implement ETH as an alternative collateral asset. The team is targeting a launch in early 2020 and the community is hoping that the initiative will extend the system’s throughput and make the service more accessible. 

## The Situation

My first reaction when I heard about the ETH collateral proposal was a visceral rejection. Adding ETH as an alternative collateral asset would introduce unknown complications into the system, while diluting the value of my SNX investment. <a href="https://twitter.com/binance/status/1114027659015544832?s=20" target="_blank" class="link">*But muh bags.*</a>

The deeper I delve into the mechanics, however, the more my opinion has turned. Not only do I now support ETH as collateral, I believe it may be essential to the success of the project. 

While the team is rolling out a slew of protocol enhancements over the next six months that will draw in new users and elevate the platform’s competitiveness, there *is* some useful and informative data we can glean from the early days. The first and simplest data point is the distribution of staking rewards over the last few months as the project has entered the crypto mainstream. Rewards are still weighted heavily towards SNX, a yield stream that will taper off significantly over the next few years. 

sUSD rewards &#8722; the other source of staking yield &#8722; have been volatile since September, the spikes owing partly to front-running bots that the team has been working to engineer off the platform. We’ll discuss why staking rewards are pertinent to the ETH Collateral debate later on.

> These are *my* estimated returns over the time period. Based on a variety of factors, others’ numbers might be a bit different.

<img class="blog-img" src="/docs/assets/eth-collateral/weekly-rewards.png">

While no one would suggest that sUSD trading rewards over the last few weeks (very low) &#8722; or the few weeks prior (very high) &#8722; represent the run-rate yield of the system, maybe the right answer is somewhere in between. However, before we can consider potential run-rate returns, we need to establish some key metrics for evaluating trading activity on Synthetix.

## Understanding Trading Yield

This blog post is not about valuing the SNX token. That said, some SNX valuation models use a conventional DCF analysis &#8722; based on growth assumptions in exchange volume and fees &#8722; to determine a fair value...there’s nothing technically wrong about this approach, but I think it misses a key point. 

Take the simplified example below. At a $1.50 token price, the network liquidity is capped at $22.5 million. Over the course of the year, investors rack up 6% of capital in fees. In this environment, SNX stakers earn a total 0.8% pre-debt trading yield on their holdings. 

At the beginning of year 2, demand for liquidity on the network grows by 2%. The price of sUSD briefly increases to $1.02, before investors bid up the value of SNX by 2% in order to print more liquidity. At the end of year 2, the token has appreciated by 2%, but the trading yield has stayed exactly the same. 

<img class="blog-img" src="/docs/assets/eth-collateral/demand-growth-example.png">

An increase in demand led to growth in capital but not growth in yield. While token appreciation is an important part of the returns equation for early holders, the trading yield needs to be competitive with other cash flow generating assets for the project to be sustainable long term. That’s why a DCF that only considers growth in exchange volume doesn’t paint the full picture.

> Token capital returns exist on a separate risk-reward axis from trading yields. In the former, an investor is betting on growth in demand for the platform vs. the possibility of growth declining. In the latter, stakers are betting on a yield sufficient for the risk of assuming trader debt. 

So if a raw increase in demand for the network doesn’t move the needle on yield, what does? The operative metric is something we can call `trading velocity`. 

**For each dollar of liquidity minted to the network, how many times a year does it generate fees?**

So how do we estimate velocity? Synthetix Exchange has been around for almost exactly a year, making it easier to build a simple model for trading velocity.  The takeaway from the exhibit below is that one dollar of liquidity turned over about 26 times in the past year, controlling for inorganic activity from front-running bots. Said another way, the network’s liquidity enters and exits an average of 13 trades per year.

To estimate the run-rate velocity, I've increased my estimate for historical velocity by 25% to account for the fact that the network’s liquidity has been underutilized in year 1. This is most evident in the fact that the sUSD peg has struggled to maintain parity with other USD stablecoins. (The values in green are real and the values in blue are my assumptions.)

<img class="blog-img" src="/docs/assets/eth-collateral/run-rate-velocity.png">

> The best metric we have for knowing whether the network is at capacity is the status of the peg. If it’s below $1, the network is underutilized. If it’s above $1, the market will bid up the price of SNX and stakers will mint more liquidity, pressuring the spot back down to $1. 

With the trading velocity in hand, we can estimate what the current run-rate yield is for SNX. **This is the annual return that stakers will expect in exchange for taking the other side of *every* trade.**

Under our assumptions for C-Ratio, velocity and fees, the run-rate yield is only about 1.3% annualized. Because 32.6x is a very rough estimate, I’ve included a range to gauge the effect of higher or lower velocity. But in any case, these yields are not sufficient to take on global trading risk.

<img class="blog-img" src="/docs/assets/eth-collateral/current-trading-yield.png">

Fortunately, we would expect this estimate to grow as Synthetix moves beyond vanilla synths trading and introduces more profitable products in the futures and derivatives space. Additionally, it’s possible that once the front-running kinks are worked out, the average trader will be net unprofitable, especially if Synthetix finds product-market-fit as a hedging utility. Lastly, dynamic fee models should make certain products (like forex trading and swaps) more competitive. 

However, something in the ballpark of 1.3% won't be sufficient to support a healthy cash flow generating asset. At some point, trading yield &#8722; not growth &#8722; will start to drive token price. Even if we’ve under-estimated trading velocity by a factor of 2 or 3, it may not be enough to compensate holders for taking on the risk of global debt. And as we established earlier, growth in liquidity is not correlated with growth in yield.

So how do we support a healthy trading yield? 

## Ether Collateral

Let’s do some math on what adding Ether as a collateral option could mean for fees. Recall, only SNX stakers collect fees. sETH minters do not. 

If we assume that Ether collateral will be capped at 50% of SNX collateral and that the average C-Ratio is 150%, traders will be able to mint an incremental ~$56 million in sETH. That's significantly more fee-generating liquidity paying the same number of SNX holders.

<img class="blog-img" src="/docs/assets/eth-collateral/minted-seth.png">

> The ETH collateral cap will be much lower than 50% early on, but we would expect it to rise as confidence in the system grows. 

With $56 million in new Ether-collateralized liquidity, there are three potential sources of revenue. 

* **Interest fees**: while the leverage gained from SNX staking is interest-free, leverage is, after all, a loan to the trader, and interest will be charged on minted sETH. Traders are higher risk than the average CDP owner, so I’d expect a rate higher than the 5% or so currently charged to Dai minters (we assume 10% here)
* **Trading fees**: we assume the same 0.3% trading fee as for sUSD trades
* **Minting fees**: there may be a minting fee (we assume 0.5%)  to gain entry to the network. Because sETH is freely traded on Uniswap, it’s unlikely that every sETH trader will pay this fee, so we’ll assume that sETH capital only generates minting fees 2x per year.

Applying these estimates, we can expect nearly $12 million in new trading fees. 

<img class="blog-img" src="/docs/assets/eth-collateral/network-fees.png">

Finally, we’re going to assume that the growth and stability that come from Ether collateral allows the community to reduce SNX collateralization requirements to 500%, adding some extra leverage. 

**Overall, we can estimate that Ether collateral boosts our annual trading yield to nearly 9%, roughly 7x larger than the current 1.3% run-rate.**

<img class="blog-img" src="/docs/assets/eth-collateral/new-trading-yield.png">

Of course, the effects of global debt are still unknown, and they would likely vary from year to year. However, a 9% yield seems sufficient to support the asset long term. 

## To the Moon

Ether collateral brings new risks with it &#8722; a subject for another blog post &#8722; but without it, Synthetix will have a difficult time achieving its massive potential. Adding Ether injects much-needed leverage without diluting the value of the SNX token. 

Instead of thinking about SNX as the collateral asset for the network, it may be more appropriate to think of it as the base collateral asset &#8722; the foundation and backstop for the network. And while a change of this significance will come with its fair share of challenges, the path to becoming Decentralized Bitmex runs through Ether.

