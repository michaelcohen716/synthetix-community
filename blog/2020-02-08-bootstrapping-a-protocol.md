---
title: Synthetix Monetary Policy: Bootstrapping a Protocol
---
<div class="author">
<a class="link" href="https://twitter.com/mjayceee" target="_blank">@mjayceee</a>
</div>

## Background

Before DeFi was the meme and TVL was the narrative, Ethereum builders recognized the **necessity of a decentralized stablecoin**. To underpin a new financial ecosystem, this stablecoin would need to be **fiat-pegged** without relying on legacy infrastructure or centralized institutions. And to administer monetary value, it would have to be **backed by real collateral** while remaining accessible to anyone on-chain.

There was no shortage of projects trying to meet this need. However, MakerDAO, a system built on an intricate set of contracts, a progressively more robust network of oracles and an active governance model, achieved remarkable success quickly and continues to be the focal point of DeFi. In the Maker system, borrowers post at least 150% in ETH collateral to mint Dai, a synthetic stablecoin. The borrower must pay a variable interest rate and maintain a minimum level of collateral, but the coin can be spent freely &#8722; without restriction &#8722; and freely &#8722; without expense (excluding gas fees).

One of the many projects operating in Maker’s shadow was Havven &#8722; a stablecoin system with a similar goal but an alternative approach. Holders of the HAV token staked their value in order to mint a stablecoin called nUSD. There were no interest fees, but each time nUSD was transferred, the spender would pay a small fee directed to the stakers collectively collateralizing the pool. 

<img class="blog-img" src="/docs/assets/bootstrapping-protocol/nusd.png">
<div class="caption">Synthetix nUSD promotional material</div>

There are any number of reasons why one project succeeds over another, but Maker found a working model with the right timing and community support. By November 2018, it was clear that Dai was the standard-bearer for decentralized stablecoins: **outstanding Dai outnumbered outstanding nUSD by roughly 75x**. 

That November, realizing that Maker had beaten them to the spot, Havven rebranded as Synthetix and **refocused on building an *ecosystem* of synthetic assets**, rather than just one. 

<img class="blog-img" src="/docs/assets/bootstrapping-protocol/hvntosnx.png">
<div class="caption">Havven pivot to Synthetix</div>

Now, fourteen months and twenty synthetic assets later, Synthetix and its stablecoin have come full circle. As DeFi enters a new period of growth, sUSD stands as **the only credible, decentralized alternative to Dai**. 

However, this torrid pace of growth didn’t begin when the project rebranded or refocused. In fact, the turnaround was catalyzed by an ambitious and inventive approach to monetary policy that complemented the novel token model that SNX inherited from HAV. 

**Synthetix still has a long way to go until it can overtake Maker’s utility in the ecosystem**. But it’s worth reviewing the monetary policy tools that got us to this point and illuminating how monetary policy can help propel Synthetix into the top spot in DeFi.

## Staking Incentives

The SNX token model is dependent long-term on trading fees and, perhaps, a small perpetual staking incentive. But in the months after the pivot to Synthetix, trading fees were anemic and participation in the protocol was minimal. 

Drawing inspiration from Bitcoin’s monetary policy, Synthetix launched an **aggressive inflation schedule** with 75% emissions in the first year. The result was a virtuous cycle of liquidity and trading activity that catalyzed the 2019 bull run.  

<img class="blog-img" width="100%" src="/docs/assets/bootstrapping-protocol/inflation-schedule.png">
<div class="caption">Current Inflation Schedule: March, 2019 - February, 2030 &#8722; source: @deltatiger, SIP 23/24)</div>


Before staking incentives, no more than 40% of outstanding SNX supply was staked. Just months later, the number was closer to 80%. Generous rewards led to increased interest in the project which, in turn, led to an increase in the price of SNX, allowing stakers to mint more liquidity for the network. Bootstrapping liquidity is **the** challenge for many crypto projects, but Synthetix seems to have found a successful formula.

But despite the growth in liquidity, traders weren’t flocking to the project en masse. When stakers minted sUSD, many were keeping their funds in their wallets or selling them for a discount on the open market. It was clear that **bootstrapping liquidity wouldn’t be enough to jumpstart the protocol** if the liquidity wasn’t flowing freely to traders. 

## Uniswap sETH Pool
While generating liquidity was a good first step, traders still weren’t particularly interested in synths. One obvious pain point was the friction of converting ETH to sUSD to sBTC, sETH or some other synth in order to trade. As such, the team posited that the best way to **bridge the divide between Synthetix Exchange and the rest of Ethereum** was to enhance the liquidity of the ETH/sETH pair &#8722; the base reserve asset and its synthetic counterpart.

A centralized listing wasn’t on the table for a synthetic token with no volume. And an internal solution could be time-consuming and would be no guarantee to work. With that in mind, the team tapped into the **composability of Ethereum** by harnessing the power of Uniswap. 

By early July, the inflationary incentives we mentioned earlier had kickstarted liquidity on the network. The community decided to divert a small share of that inflation to <a href="https://github.com/Synthetixio/SIPs/blob/master/SIPS/sip-8.md" class="link">incentivize participation in the ETH/sETH pool</a> on Uniswap. Still today, a total of 72,000 SNX a week are transferred to the liquidity providers in the sETH pool, proportional to their contribution.

Prior to this initiative, the Uniswap ETH/sETH pool was an afterthought. It had 50 ETH/sETH or less in liquidity and wasn’t active enough to incentivize capital to flow organically. But just six months later, the sETH pool is by far the largest on Uniswap and has, at times, been worth more than the several top pools combined.

<img class="blog-img" width="100%" src="/docs/assets/bootstrapping-protocol/seth-pool.png">
<div class="caption">Growth in the Uniswap sETH Pool since September (there was one previous version of the pool) &#8722; source: Uniswap.info </div>

A deep and incentivized sETH pool serves three purposes for Synthetix:
* an easy on-ramp for traders large and small
* a more robust ETH/sETH peg
* a substantial, albeit artificial, source of demand for synths

With the sETH pool in place, the community has now bootstrapped a **key piece of foundational infrastructure** that will prove valuable for a long time. But even in the early days of the sETH pool, it was clear that deeper Uniswap liquidity only bolsters a soft peg, it doesn’t guarantee it. In the Uniswap model, the deeper the liquidity, the harder it is for traders to offset the peg. But &#8722; given a bearish trend &#8722; there’s **no guarantee that the demand will be there to restore the peg** to parity. Traders may not have wanted to enter the system if they weren't confident about exiting their synth position at full value.

## Arb Pool

Enabled by the infrastructure of the new sETH pool, the <a class="link" href="https://blog.synthetix.io/snx-arbitrage-pool/">Arb Pool</a> was designed to lift the sETH/ETH ratio when it fell below a certain threshold (i,e., when the soft peg was struggling to trade at parity). Contributors could send ETH to be converted to sETH which would be converted to SNX at parity and sent back to the user. In short, the incentive was to buy discounted SNX with ETH, which was used to stabilize the ETH/sETH peg in turn. This was funded, yet again, with another small slice of protocol inflation.

Before the Arb Pool was announced, the sETH peg was unreliable and the asset sometimes traded in the 0.80s against ETH. Synthetix’s other soft peg, sUSD, often traded in the $0.80s as well. 

<img class="blog-img" width="100%" src="/docs/assets/bootstrapping-protocol/susd-peg.png">
<div class="caption">sUSD Peg &#8722; source: Coinmarketcap </div>

But just the *announcement* of the Arb Pool mechanism sent the soft pegs soaring towards parity (July ‘19 in the chart above). Even before any incentives were in place, both the sETH and sUSD pegs were back to trading in the high 0.90s. It turns out that **a key element of maintaining a soft peg is the belief system behind it** &#8722; frankly, the confidence that someone else will be there to buy the asset at or about the same price. 

For awhile, the Arb Pool was quite successful, serving as a buffer for the soft peg when it began to deteriorate. Early on, the mechanism was manual &#8722; someone would send proof of their transaction and would then be sent discounted SNX. Eventually, the team formalized the process with an automated contract that was filled with SNX every week.

But, as is common in the adversarial world of crypto, someone found an exploitable flaw in the system. In recent months, larger traders have knocked the peg off intentionally (by selling sETH in size) to benefit from this incentive, quickly draining the weekly allocation of SNX. Somewhat counterintuitively, **the manual process may have been more efficient than the automated one**. The community decided to sunset the Arb Pool and is now experimenting with a new auction model for raising ETH.

## Challenges Ahead

These three initiatives have vaulted Synthetix into the conversation as one of the most exciting projects on Ethereum. But each element of the Synthetix monetary policy &#8722; 1) incentivizing staking, 2) subsidizing sETH liquidity and 3) defending the sETH peg &#8722; relies on an inflationary curve that will decline to 2.5% annual by 2024. Simply put, **the funding for these initiatives will no longer be available in the not-so-distant future**. So how can Synthetix &#8722; its influence on the Ethereum ecosystem dependent on the success of the sUSD stablecoin and the sETH soft peg &#8722; ascend to the zenith of DeFi?

## Sunsetting Inflation
Will stakers and token holders remain engaged once staking incentives dwindle? Well, in some sense, that’s the existential question for Synthetix. By the time we reach terminal inflation in 2024, the team will need to have executed on a competitive product that generates enough fees to cover the risk of staking. **The inflation schedule serves as a natural timeline for the team and the success of the project**.

What about the sETH pool and its goal of providing an easy on-ramp to Synthetix Exchange? With the introduction of ETH collateral in the coming weeks, this problem may actually solve itself. There will always be a Uniswap pool (and hopefully a Curve pool and dex.blue listing soon, as well), but once traders are staking ETH as collateral to trade, they’ll actually be staking *their own* entry and exit liquidity. As ETH-collateralized liquidity becomes a larger part of the activity on the network, a more natural, non-incentivized secondary market for sETH will develop as well.

## Protecting the Peg
As inflation-funded capital dries up, protecting the two Synthetix pegs with an Arb Pool or an auction will no longer be an option. But in more advanced stages of the project, should we even need artificial &#8722; and expensive &#8722; mechanisms to maintain a stable peg?

Stepping back for a second, **a “stable” peg is just a relative balance between supply and demand**. If sETH and sUSD are stable, it suggests that the amount of synths in the ecosystem is roughly sufficient to meet demand. 

A good Synthetix product is the main determinant of demand. And while of course a competitive product is ultimately the goal, short term demand is not necessarily within the team’s control. **The main determinant of supply**, however &#8722; the minimum collateralization ratio for stakers &#8722; **is very much a lever available to the community**. After all, the current ratio of 750% is mostly arbitrary. After a trial C-RATIO of 500% where supply was clearly too easy to come by, the increase to 750% has worked well as a placeholder for a growing project. But at some point, **C-RATIO will be the only viable lever to ensure the integrity of the peg**.

## Being More like Maker
Maker is a complex system, but, fundamentally, there is only one key moving part: the interest rate charged on borrowed Dai. When the spot price falls below the $1 peg, MKR holders will often vote to raise the “stability fee”, encouraging borrowers to pay back their loans and burn excess supply. When the price rises above the peg, the fee will be voted lower, encouraging growth in supply. This is a simplification of MakerDAO, but interest rate policy is the central element of the system’s governance.

And Synthetix should take note. **The success of the Maker project can be traced to a nimble governance framework**. It wasn’t that long ago that Dai was struggling to maintain $0.90. Yet, after several aggressive increases in the stability fee, the peg was restored.  

There’s some resistance in the Synthetix community to a more dynamic C-RATIO. Some think that more frequent changes would make the staker experience unwieldy. Others think that frequent changes would be bad PR. There may be morsels of truth there, but the current solutions are artificial and unsustainable. Adjusting the C-RATIO calibrates supply to demand without costing the protocol a small fortune in SNX per week. And with declining inflation cutting into available capital, **C-RATIO adjustments will soon be the *only* tool available to maintain the peg**. 

> There are discussions to change the rewards claim period from two weeks to one. If this is implemented, C-RATIO adjustments will be even more effective as stakers will be forced to fix their ratios more quickly in order to collect dividends.

After some early challenges, novel monetary policy has catapulted Synthetix into the conversation with Maker. While Synthetix has some natural advantages over Maker in the battle for ETH collateral (blog post forthcoming), **the community should consider learning from the governance that has made Maker so successful**. Monetary policy has gotten us this far, and if sUSD is to one day overtake Dai, constructive monetary policy will have played a pivotal role. 