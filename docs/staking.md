---
id: staking
title: Staking FAQs
sidebar_label: Staking FAQs
---

## Why does my total debt fluctuate over time? 

When you stake SNX and mint sUSD, you create a 'debt,' which is how much sUSD you need to burn to unlock your SNX again. Your debt represents a proportion of all the debt in the system. Whenever someone makes a gain through Synths, they make it against all the debt in the system. Therefore, if the system debt increases, your debt will proportionately increase as well. 

When you mint sUSD, the Synthetix smart contract will work out how much debt you represented in the network at the time you joined. For example, if you minted $1000 sUSD and the total sUSD value of all Synths in circulation is currently $1 million, your debt ratio owed to the network is 0.1%. However, as the total sUSD value of Synths increase (such as when sBTC or sETH increase in value), your debt ratio owed to the network remains constant at 0.1%. Imagine if total sUSD value of all Synths suddenly doubles due to price increases in Synths such as sBTC or sETH, and now gets to $2 million, you will need to repay $2000 sUSD in order to unlock all your SNX.

Why does this happen? This is because every staker needs to share the debt in proportion to their initial ratio so that the monetary policy balances out. There is no free money created out of thin air. Every sUSD gain generates a corresponding debt value. 

**A detailed example:**

There is $50k of sUSD in circulation, which represents the total value of all Synths. You then stake your SNX and mint $50k of sBTC (10 sBTC worth $5000 sUSD each) so there's now $100k in total worth of Synths. So, now we have 50k sUSD and 10 sBTC. Now the price of sBTC doubles. There is now 150k in the network in sUSD. So you want to leave. At the time you joined your proportion of the debt was 50%. So you are responsible for 50% now, which is $75k USD. But BTC is $10k, so you will need 7.5 sBTC to exit. This would leave you with 2.5 sBTC free.

WAIT! Where did that 'free money' come from? The answer is that the total debt of the other SNX stakers, the ones who supplied the sUSD, went up by 50% from $50k sUSD to $75k sUSD. So now they will need to burn that much to unlock their SNX. 

## How do I increase my C-Ratio (Collateralisation Ratio)?

If your C-Ratio is **below** the Target Collateralization Ratio (currently set at 800% Collateral at this of this article), you will be blocked from claiming rewards and you will need to increase your C-Ratio to claim. 

You can increase your C-Ratio in two ways:
- Burning sUSD
- Buying more SNX and mint more sUSD.

If your C-Ratio is **below** the Target Collateralization Ratio, you will be blocked and unable to claim your fee rewards. 

If your C-Ratio is **above** the Target Collateralization Ratio, Mintr will display your status as 'Good' and you can then:
- Do nothing. Continue to receive fees against your existing minted sUSD
- Mint more sUSD. To receive a greater proposition of fees in the next fee period.
- If you choose to mint more sUSD, you may want to leave a buffer of sUSD to accommodate market fluctuation of the SNX price.

Your Collateralization Ratio must be above the Target Collateralization Ratio to be able to claim your fee rewards. 

## I previously locked my SNX to mint sUSD. How can I unlock my SNX?

To unlock your locked SNX, you need to 'burn' the sUSD you debt owed. Burning will unlock your escrowed SNX first then it will start unlocking your SNX in your wallet to transfer.  

If you had $1000 worth of SNX you would have been able to mint ~133 sUSD (at the 750% Collateralization Ratio). This would lock up all of your SNX, thus making it non-transferrable. You cant mint money then sell your collateral used to supply it. The minted amount must be burned. 

So you now need to burn that 133 sUSD you minted (give or take any fluctuations in your debt) to unlock your SNX so you can transfer it. Mintr will tell you how much sUSD you need to burn to unlock your SNX.

**What if I don't have any sUSD in my wallet to burn?**

If you have an sUSD debt but you have no sUSD in your wallet then you must have done one of the following:
- Transferred it to another wallet
- Transferred it to an exchange and sold it
- Sent it to the Depot to be purchased via Synthetix.Exchange
- Exchanged it into another Synth on Synthetix.Exchange

To unlock your SNX, you must acquire the amount of sUSD under Debt in Mintr. If you transferred it to another wallet or an exchange, you will need to transfer it back into the wallet that contains your locked SNX. And if you sold the sUSD, you must buy it back. 

You can purchase sUSD easily from [Curve](https://curve.fi} or [Uniswap](https://uniswap.exchange). 

Once you've paid back your sUSD debt, your SNX will be unlocked and able to be transferred. 

## I claimed my SNX staking rewards but I don't see them in my wallet

When you "claim" in the Rewards tab on Mintr you are assigned your % of SNX in an escrow record in the RewardEscrow Contract. Your rewards will not show in your wallet address but they are assigned to your wallet address to be vested in 12 months from their claim date.

You will now be able to mint from those escrowed SNX as they are also used as your collateral. So mint away if you can and compound your next weeks SNX rewards. 

## Why does the number of my staked SNX fluctuate? 

If you've staked your SNX, you might have noticed that the number of staked SNX in your wallet can change. This is due to fluctuations in the SNX price. If you stake your SNX at a 750% Collateralisation Ratio, and the SNX value increases, then your C-Ratio will increase and some of your SNX will be unstaked. This is because only enough SNX to cover a 750% ratio will be staked. But then if the SNX value decreases, and your C-Ratio goes back to 750%, all of your SNX will be staked once again. 

If your C-Ratio is above 750%, you can always choose to stake the rest of your SNX by selecting 'Mint Max.' This will increase the number of staking rewards you are entitled to receive. 

## How can I check exactly how many of my SNX are unlocked?

If you try to send more SNX than you have "transferrable" then the transaction will fail. The easiest way to check how many SNX are unlocked is on Mintr in the following screen: 

<img src="static/img/unlockedSNX.png">

## How can I delegate claiming rewards, minting, or burning to another wallet? 

The full process is outlined in detail [here](https://blog.synthetix.io/a-guide-to-delegation/).

## Now that I've staked SNX and minted sUSD, what can I do with it? 

Firstly, there is [Synthetix.Exchange](https://synthetix.exchange), which is a trading platform allowing you to trade your sUSD for any of our synthetic assets (Synths). It currently supports a variety of forex currencies (e.g. sEUR), cryptocurrencies (e.g. sBTC), indices (e.g. sFTSE), and assets (e.g. gold/ounce as sXAU). The best thing is, there's no slippage and it doesn't require a counterparty, so there's no waiting around for your trade to get filled. So for example, if you'd like exposure to Bitcoin without leaving Ethereum, you can trade your sUSD for sBTC on Synthetix.Exchange. 

Secondly, you can sell it on somewhere like [Curve](https://curve.fi} or [Uniswap](https://uniswap.exchange). 

Thirdly, you can lend it out on a lending platform such as [AAVE](https://aave.com). 

Keep in mind if you choose any of these options that you'll need to burn enough sUSD to cover your 'debt' if you want to unstake your SNX. 

## How can I stake SNX and receive staking rewards?

In February 2019, we provided a [long explanation](https://blog.synthetix.io/synthetix-monetary-policy-changes/) of why we decided to change the total SNX supply over the next five years from 100,000,000 to ~260,000,000, after which there will be an annual [2.5% terminal inflation for perpetuity](https://blog.synthetix.io/reaching-monetary-policy-consensus/). The primary reason is to increase greater incentive for SNX holders to stake their SNX and mint Synths, and the schedule is designed to reward early contributors. 

The way the SNX staking rewards work is that holders who have staked their SNX and keep their Collateralisation Ratio at or above the target receive a portion of the additional SNX added to the supply. Rewards are distributed weekly to be claimed by SNX holders the following week. 

**Fee Claim: Blocked Status**
Rewards and Fees are blocked from being able to claim if you are below the target C-Ratio. To unblock claiming your rewards, you must burn enough sUSD to get to the target.
