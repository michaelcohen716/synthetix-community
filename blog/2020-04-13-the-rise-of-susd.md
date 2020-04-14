---
title: The Rise of sUSD
image: /docs/assets/rise-of-susd/stablecoins.png

---
<div class="author">
<a class="link" href="https://twitter.com/mjayceee" target="_blank">@mjayceee</a>
</div>

## Background
Inside the crypto ecosystem, nothing paints a clearer picture of the philosophical and technical contrast between centralized and decentralized &#8722; or permissioned and permissionless &#8722; more than stablecoins. At this stage, even the most virulent maximalist would admit that stablecoins are critical to the success of crypto. But, while the utility is crystal clear, the methods and the values underlying each system are a constant source of contention. 

The blunt irony is that the stablecoin industry is hella volatile. 

Tether (USDT) is the clear leader in adoption with nearly 10x the market cap of its nearest competitor. While USDT is a fiat-backed stablecoin, <a href="https://www.bloomberg.com/news/articles/2019-04-30/tether-says-stablecoin-is-only-backed-74-by-cash-securities" target="_blank" class="link">it may not have been always been backed by fiat</a>. Still, it's a useful vehicle for transferring value and holders are at peace with past controversy. Liquidity begets liquidity and traders have adopted Tether as their stablecoin of choice. 

<!--truncate-->

But the shortcomings of Tether &#8722; **questionable collateral-backing and outright centralization in the hands of an exchange operator** &#8722; are anathema to true ETH believers and the risk-averse alike. Circle’s stablecoin (USDC) is ascendant as a safer, fiat-backed option for traders, commercial partners and DeFi users. USDC is backed by a more trusted exchange operator in Coinbase and at least <a href="https://www.centre.io/index.html" target="_blank" class="link">makes an attempt at embodying the ethos of decentralization</a>. 

As you scroll down the stablecoin leaderboard, there’s a laundry list of undifferentiated centralized, fiat-backed competitors. Interrupting the lineup at #6 overall, however, is DAI, the leading decentralized stablecoin. DAI is backed by MakerDAO smart contracts and (mostly) Ether collateral making it the top choice for many DeFi users. **Maker is the focal point of DeFi and undoubtedly the most impactful project in the space**. But, even before the events of Black Thursday, the project has always attracted a great deal of criticism, a trend that is only accelerating. 

<img class="blog-img" src="/docs/assets/rise-of-susd/stablecoins.png">
<div class="caption">Some of the stablecoin players</div>

**Every month, it seems, there’s a new flavor of alternative**, poised to challenge DAI’s hegemony. For a while, many were pushing for a fork of Single Collateral DAI, Maker’s original, simpler iteration. More recently, projects like MetaCoin and mStable &#8722; intricately configured baskets of existing stablecoins &#8722; have arrived on the scene with their own perspectives on the weaknesses of the current paradigm. MetaCoin’s thesis is that many prefer a stablecoin with minimal governance, backed solely by ETH. mStable’s thesis is that the stablecoin space has become too fragmented to function practically.

All of these are likely viable in some way. But my question is this: Why are we forking massive codebases or building abstractions on abstractions when a permissionless stablecoin backed by permissionless collateral already exists? **Why are we trying to build an alternative to a project flirting with centralization when a crypto-native stablecoin with a path towards decentralization already exists?**

Look no further, folks. sUSD is perfectly positioned for this moment in the evolution of DeFi. DAI isn’t going anywhere anytime soon, but it’s **time to elevate sUSD as the permissionless alternative** with the foremost commitment to the values of decentralization. 

It’s not just the principles of it, though. sUSD in its current form is **structurally more sound** and, most importantly, **a lot more useful** than DAI. 

## The Missing Gear

Maker is a clever system: levers and pulleys designed to maintain a soft peg without coercion. A combination of monetary policy and arbitrage opportunities drives the peg towards $1 in either direction. But, during a period in March 2019 when the peg was drifting slightly, Twitter user and DeFi whisperer @DegenSpartan highlighted a <a href="https://twitter.com/DegenSpartan/status/1103189312529620993" target="_blank" class="link">subtle crack in the arbitrage model</a>. 

When the peg is under $1, the Maker system theoretically incentivizes CDP owners &#8722; the users who have leveraged their ETH collateral to mint DAI &#8722; to buy back the stablecoin at a discount to repay their debt below cost. However, this mechanism wasn't quite working that March, and to understand why, we need to remember that the most common type of CDP user is someone who is long ETH and wants to lever up using DAI. At this stage in the market cycle, the market sentiment was overwhelmingly bullish. Unfortunately for the peg, **a couple cents of arbitrage wasn’t enough to encourage enough traders to unwind their positions**.


There are always some arbitrageurs waiting in the wings, but at some point the overlap between CDP owners and traders positioned to perform arbitrage disappears. And the equilibrium price where this occurs could very well be 96 or 97 or 98 cents. 

> To be fair to Maker, there's an argument to be made that the minting of DAI will become institionalized in such a way that large investors like Paradigm will be responsible for an outsized share of liquidity. As major minters, they'll take on the burden of performing arbitrage at the tempo necessary to maintain a strong peg, as it's in their financial interests as MKR holders. 

___

Now, this design flaw is just a minor blemish. It doesn’t really diminish DAI’s status as the linchpin of DeFi. Whether via more aggressive monetary policy or an eventual arbitrageur, the gap will be filled. 

However, this hole in the arbitrage model exposes a much larger structural flaw in the Maker model: as @DegenSpartan put it, **DAI supply does not scale with DAI demand**. DAI supply is primarily a function of an ETH holder’s propensity to leverage their position.

Herein lies the critical flaw: **DAI supply is largely divorced from the demand for decentralized stablecoins**. There’s a non-trivial group of CDP holders who borrow against their ETH to pay for expenses, sure, but none of these investors have a bearish view on ETH. If they did, 1) they’d be committing themselves to re-collateralizing their CDPs at a later date or 2) they would just sell their ETH for DAI or USD. 

This conundrum was known to <a href="https://medium.com/reserve-currency/our-analysis-of-the-makerdao-protocol-4a9872c1a824" target="_blank" class="link">researchers in the space as early as 2018</a>, but DAI has been the only real game in town since it launched. Synthetix’s predecessor, Havven, made a valiant attempt to mount a challenge, but it wasn’t until more recently that the pieces have come together to make sUSD a viable competitor. 

## Scaling Supply with Demand

Before we go too deep, let’s examine a simple example of how sUSD supply scales with demand. In the exhibit below, there is $2.5 million of demand in the market for sUSD and $12.5 million in total demand for synths. Over a period of time, sUSD demand grows by 10% to $2.75 million while other synth demand remains the same. All things equal, **the market will recognize that the demand for synths isn’t being met** at the current price of SNX and **investors will bid up the value** to increase stakers' capacity to mint. In this case, the price of SNX rises by 2%.


<img class="blog-img" src="/docs/assets/rise-of-susd/demand-increase.png">


How does the market recognize that it’s time to bid up SNX? Likely, some combination of the sUSD or sETH pegs trading at a premium, and/or synth yield opportunities becoming more attractive to potential minters. You’ll notice that **these are both demand-side motivations**. The market signals that more synths are desired, and stakers &#8722; eager to earn as much in trading fees as possible &#8722; are motivated by profit to create synths and inject them into the market. 

> Recall, staker rewards are determined by dividing total trading fees in a period by the staker’s proportion of global debt minted to the system. So, many stakers will mint as much as the collateralization ratio allows for.

The key takeaway here is that if investors, consumers or DeFI users want to hold or transact in sUSD, the SNX ecosystem will meet that demand. On Black Thursday, when DAI liquidity was nowhere to be found and ETH prices were in freefall, **there was no clear mechanism within Maker to generate DAI**. So, Maker took the unfortunate step of introducing a centralized asset &#8722; USDC &#8722; as collateral to increase liquidity and lure in arbitrageurs. Liquidity started to flow and the peg eventually recovered but, really, it was too late: <a href="https://medium.com/@whiterabbit_hq/black-thursday-for-makerdao-8-32-million-was-liquidated-for-0-dai-36b83cac56b6"  target="_blank" class="link">the keeper market broke down and millions of dollars in ETH were effectively stolen from CDP holders</a>.


## sUSD Beats DAI at its Own Game

**In its current form, Ether collateral on Synthetix isn’t all that useful for traders who want to lever up their Ether position**. That’s because ETH collateral allows traders to mint sETH debt at a 150% C-RATIO. The drag is that a trader is trading against the price of ETH. In an ecosystem made mostly of long term crypto bulls, this is an especially unattractive proposition.

In the example below, a trader mints sETH using ETH collateral and seems to make a profitable sLINK trade in USD terms. But when the debt comes due, the trader is actually in the red, because ETH outperformed in the meantime.

<img class="blog-img" src="/docs/assets/rise-of-susd/eth-collateral.png">

So, right now, trading with leverage on Synthetix isn’t all that attractive. As a means to obtaining leverage on an ETH position, Synthetix is not yet in competition with Maker.

However, in an upcoming release, **Synthetix will introduce sUSD-denominated ETH collateral** &#8722; a feature familiar in many ways to Maker CDP owners &#8722; and **the value proposition will flip overnight**. Not only will this feature deliver more utility to the trader, it will also expose a key advantage sUSD has over DAI as a stablecoin.

First, the newly minted sUSD will be many times more powerful than DAI. **sUSD has a native use case in the Synthetix system without comparison in Maker**. A trader can sell that sUSD for ETH, just like a CDP holder might. Or &#8722; this trader can sell sUSD for sBTC, sETH, iTRX, sFTSE, sGBP or any of the other ~30 synths currently available on Synthetix. Even in the most DAI-like scenario where a trader uses sUSD to lever an ETH position, traders on Synthetix will soon have 5x, 10x and greater leverage opportunities available natively with their sUSD. 

**Put another way, sUSD is poised to appropriate DAI’s foremost use case. And when the dust settles, the utility gap will have been blown open.** 

Just to rub salt in the wound, the sUSD peg is far better equipped than DAI to absorb the massive issuance that comes with traders generating leverage. When CDP owners mint DAI to buy more ETH, they’re immediately selling DAI back on the open market. As they build leverage, more and more DAI floods Uniswap and Oasis, driving the peg below $1. As we discussed earlier, there are few natural buyers here except for the cadre of traders willing to sit on their hands waiting for the peg to rebalance.

And in sUSD’s case? When a trader converts sUSD to sETH or sBTC or iETC on Synthetix Exchange, the system burns it. It no longer exists. **When traders deploy their synthetic capital, the peg grows stronger**. 

> Synthetix's ecosystem of synthetic assets would also have theoretically proved useful on Black Thursday. If sUSD is the stablecoin of choice the next time the market plunges, sUSD-denominated ETH-collateral borrowers will be able to convert any funds floating in the 30+ outstanding synths into sUSD to pay back their debt. This a major contrast to the experience of competing for overpriced DAI on the open market. 

## The Transition Begins

Of course, DAI (Multi-Collateral DAI) is still about 15x larger in market cap and many multiples larger in mindshare. But it’s difficult to observe the trajectory of each project and not come to the conclusion that **DAI and sUSD are at least equally positioned in the decentralized stablecoin space**. 

The events of Black Thursday &#8722; when Maker stumbled through a stress test &#8722; exposed some fairly consequential weaknesses in the system. Synthetix isn’t perfect, but Black Thursday proved that we need a decentralized alternative to DAI. Over time, the alternative may prove to be the replacement.
