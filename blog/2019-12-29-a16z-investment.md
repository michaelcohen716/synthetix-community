---
title: What Can We Learn from the a16z Investment?
---
<div class="author">
<a class="link" href="https://twitter.com/mjayceee" target="_blank">@mjayceee</a>
</div>

## Background

The a16z investment is a bit of a mystery in the Synthetix community. It’s small for a megafund like a16z, but big enough to be taken seriously. It was unannounced and remains undeclared, yet a16z’s 374,111 SNX tokens are right there on the public ledger in the same wallet as the firm’s much larger and well-publicized MKR investment.

<img class="blog-img" src="/docs/assets/a16z-investment/a16z-wallet.png">

There’s a <a href="https://twitter.com/lawmaster/status/1185068817048838145?s=20" target="_blank" class="link">very unlikely conspiracy theory</a> on Crypto Twitter that someone sent tokens to a16z to pump the price of SNX, but as far as I can tell, a16z’s somewhat larger and less flashy investment in Augur’s REP tokens was also unannounced. That's probably just how the fund operates for positions of a certain size. While SNX investors would eagerly welcome a bullish press release, a16z’s silence over its investment isn’t all that noteworthy. 

What interests me isn’t *why* a16z hasn’t announced its SNX investment; what interests me is the nature of the investment itself. **It’s been over two months since SNX showed up in the a16z wallet, and the firm has yet to stake one token.** 

<!--truncate-->

For those unfamiliar with the project, `staking` is the process of converting SNX tokens to collateral and `minting` liquidity for the traders on the network. Stakers earn fees, while passive investors can only profit from growth in the price of the token.

The staking incentives that the team implemented in March 2019 were the catalyst for the recent bull run, and roughly 80% of SNX tokens are currently staked &#8722; up from less than 40% before the new monetary policy was enacted. In the middle months of 2019, stakers were earning annualized returns in excess of 100%.

I did some back-of-the-envelope math based off my own returns since the a16z position was opened in mid-October, and &#8722; had the firm been staking &#8722; a16z’s SNX stack would already be about 6% taller. Though SNX staking incentives have begun to moderate, it’s safe to say that **a16z could have expected compounded returns of 30-40% in the first year of its investment &#8722;** this *before* considering sUSD trading fees or appreciation in the value of SNX.

So why would the firm be sitting on the sidelines like this, at the expense of their bottom line? While most investors are cashing in on Synthetix’s <a href="https://blog.synthetix.io/synthetix-monetary-policy-changes/" target="_blank" class="link">generous early-bird protocol incentives</a>, why is a16z foregoing easy yield and allowing its position to be massively diluted?

## My Best Guess

The weekly cycle of staking, minting and claiming is an active process for SNX holders. It’s not overly involved, but it does require a decent amount of time and attention. It’s possible that it simply isn’t worth it for the team at a16z to devote meaningful effort towards actively managing an investment worth less than 1% of their fund.

This *could* be the explanation, but the firm’s wallet is a simple external address &#8722; not a multisig &#8722; and it’s hard to believe that they couldn’t establish some simple process to submit two transactions per week. The firm has recently begun participating in Maker governance votes from the same address. While MKR is a much more important investment to the firm, I don’t think that apathy is the motivating force here. 

I worked through a couple more possible explanations:
* the firm isn’t comfortable taking on the **debt risk that comes with staking**
* the firm isn’t comfortable having part of its position **escrowed** (SNX staking rewards are escrowed for one year)
* the firm doesn’t want to **manage a portfolio of synths**
* some element of the firm’s **agreement with LPs precludes staking**

All of these are plausible, and several factors may have contributed to the decision not to stake, but one alternative explanation makes the most sense to me:

***a16z and their investors don’t want to pay taxes.***

## Taxes and Fund Management

SNX investors come from countries all over the world, each with their own tax rates and frameworks, so there’s no community aspect or universal experience. By and large, taxes are not a favorite topic of conversation in the Synthetix Discord or among crypto types in general. 

But that doesn’t mean that tax considerations aren’t important to sophisticated U.S.-based investors. sUSD trading fees are definitely taxable. And SNX staking incentives are almost certainly taxable as well (although <a href="https://www.investopedia.com/terms/n/nontaxable-distribution.asp" target="_blank" class="link">there’s some case</a> to be made that they shouldn’t be). Funds managed by <a href="https://www.bizjournals.com/sanjose/news/2018/06/25/andreessen-horowitz-300m-crypto-fund-katie-haun.html" target="_blank" class="link">former federal prosecutors</a> aren’t taking chances. 

Had a16z staked their tokens, each week’s fees and rewards would trigger a tax liability for the fund’s LPs. There’s nothing wrong with a profitable fund delivering a tax bill to its investors. In this case however, **there’s no cash profit &#8722; no real distribution to LPs**. There’s only unsold or escrowed, moderately illiquid crypto sitting in an a16z wallet. 

Worst of all, income from staking would likely be taxed at the higher regular income rate &#8722; not the capital gains rate. If the firm were to stake, they might have some disgruntled, tax-liable, cash-short investors on their hands.

So now that we know more about why a16z and other similar investors may not be staking, where do we go from here?

## Considering the SNX Token Model

Like most of us, a16z is invested in SNX because they hope that the token will appreciate in value. But, at some point, trading yields will be the primary source of return for investors. If the tax rate on trading fees in a given country is 25%, SNX tokens will be worth ~25% less to that country’s investors relative to those in zero tax domiciles. **Over time, it’s not hard to imagine an investor base that migrates predominantly to low or zero tax countries in regions like the Caribbean and East Asia.** 

This may be totally fine in the long run. One of the groundbreaking features of crypto is that capital is permissionless and free-flowing. Efficient markets suggest that capital should flow to where it’s best allocated. Maybe an investor base determined by local tax treatment would work. But it *does* leave a lot of institutional capital on the sidelines. 

***Can the token model be modified to be more inclusive?***

An obvious potential solution is moving to a buy-and-burn model. Some investors and analysts are skeptical of this approach, but not all buy-and-burn models are created equally. For a token like MKR, you can trace cash flows and model valuation transparently. For a token like BNB, however, investors *may* be able to model burn rates, but they’re mostly subject to the unpredictable strategic whims of the Binance management team. 

The Synthetix variant would fortunately be more like MKR than BNB, although that doesn’t mean that moving to a buy-and-burn model wouldn’t be unfortunate. Weekly trading yields allow investors to allocate capital at their discretion. Buy-and-burn models take those decisions out of investors hands. 

But maybe it’s the *least wrong* long-term answer for a token like SNX…

Or maybe not…

**A basic analysis suggests that, all things equal, a buy-and-burn model would lead to exactly zero value accrual to SNX holders.** In the exhibit below, half of network liquidity is traded in some period and the system buys and burns SNX on the open market. The demand for liquidity doesn’t change and the number of staked SNX tokens doesn’t change, so there’s no downstream effect on price.

<img class="blog-img" src="/docs/assets/a16z-investment/buy-and-burn-value.png">

A common criticism of Synthetix is that the token model is “circular” and that the system is self-referential. Using the fees generated by the liquidity minted by the collateralized token to buy back and retire those tokens would validate that critique. **Even worse, this model would provide exit liquidity to non-stakers with the fees generated by  risk-taking stakers.** 

You could reasonably argue that there’s a flaw in the analysis above &#8722; that the reduction in total supply over time would force the price of SNX higher. This may be true. Nonetheless, it seems unwise to reduce the floating (non-staked) supply of a token that is already dubiously liquid. 

Lastly, in the event that global trading debt rises (i.e., traders are net profitable), stakers need access to capital to cover debt and unlock their SNX. In the current model, stakers can use trading fees to cover that extra debt. But if sUSD rewards are automatically redirected towards buybacks, stakers would need to draw in external capital to reclaim their SNX. Rational behavior suggests that they *would* pay off their debt to recoup their tokens, but it’s poor Investor Experience™ nonetheless.

To summarize, a buy-and-burn model perversely rewards non-stakers while the value accrual to stakers is unclear. Additionally, buy-and-burn may exacerbate the liquidity issues common to stakeable tokens, while introducing several other unwanted side effects. We can safely rule out this model as the appropriate solution to our tax problem. 

## Where Do We Go from Here?

Clearly, there’s no simple or obvious solution. Novel tokenomics naturally bring a new set of challenges and complications. 

There’s hope that SNX staking incentives will benefit from more favorable tax treatment once regulators and lawmakers provide more clarity on crypto assets. Protocols are not corporations, but SNX incentives are quite similar to equity distributions &#8722; non-taxable events in the U.S. 

It’s difficult to imagine a future where sUSD trading fees aren’t taxable, but we can hope that they’ll be interpreted as dividends and taxed at the capital gains rate. 

Is that the best we can hope for, though? That crypto protocols like Synthetix will eventually take on the same capital structures as their legacy counterparts. 

One thought (h/t @Spreek) is that divergent tax rates will induce a **lending market for SNX**, where higher tax would-be stakers will lend out their tokens to lower tax investors. Interest income doesn’t benefit from favorable tax treatment, but an interest-bearing model similar to DAI/cDAI &#8722; where gains from swapping one to the other would be recognized as capital gains &#8722; could unlock value for high tax investors. This would be a new form of `regulatory arbitrage` for the crypto age.

One more imaginative possibility would be a model where sUSD fees are diverted into an interest-generating asset pool &#8722; **our own white-labeled Compound** &#8722; where sUSD is lent out to traders. Instead of earning fees on trading directly, stakers would be granted proportional rights to the assets in the pool. Once a staker is ready to cash out, they can claim their share of the pool and pay taxes on gains. This model would give stakers more control of their portfolio strategy, while allowing sUSD rewards to compound untaxed over time.

It’s not clear whether either of these variations would fly with regulators, but it doesn’t mean that we shouldn’t start thinking about how to make Synthetix attractive to institutional investors. If the protocol is worth billions of dollars one day, professional large cap investors will have played a significant role. 
