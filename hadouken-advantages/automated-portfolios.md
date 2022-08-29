# Automated Portfolios

### **Portfolio Theory**

Pioneered by Nobel Prize winning economist Harry Markowitz in the mid-20th century, Modern Portfolio Theory (MPT) dictates how investors should choose investments to maximise overall return while limiting their risk. The most fundamental and basic aspect of modern portfolio theory is diversification. Markowitz's research showed what we know and accept today as canon, that investors can achieve the best results by choosing an optimal blend of high risk/return assets and low risk/return assets.

MPT assumes by default that investors are fairly risk-averse - as in, they prefer less risky portfolios to riskier ones, given the same expected returns. As a result, this implies that the average investor should invest in multiple asset classes. Modern portfolio theory is useful for investors who are trying to build diversified portfolios. In traditional finance, investors diversify by putting some of their assets in stocks, some into bonds, and the like. In crypto, diversification is just as easily achieved by investing in various different cryptocurrencies.

There's a fair bit of criticism on MPT, specifically that it evaluates portfolios solely on variance rather than downside risk. Meaning that two portfolios with the same variance and returns are considered equally desirable under MPT, even if one has that variance due to frequent small losses while the other has that variance due to rare but significant declines. Naturally most investors would prefer the first option. Post-modern portfolio theory (PMPT) attempts to improve on this by minimising downside risk rather than variance.

Regardless of your stance on MPT vs PMPT, or other academic approaches to constructing the ideal portfolio, it goes without saying that diversification is the best way to ensure optimal returns given a specific risk tolerance. If an investor enjoys risk - particularly due to their age or income - they might want to invest entirely in risky assets, with few strongly concentrated positions. If an investor is more on the conservative side - likely due to their proximity to retirement age - they might want to invest in less risky assets, and spread their money across various different types of assets.

Logically, as certain assets in one's portfolio increase in value - or likewise, as others decrease - portfolio rebalancing is necessary from time to time. For example, if you have a 50/50 split of two assets, _A_ and _B_, and _A_ goes up by 1000%, it might make sense to sell some of _A_ and purchase more of asset _B_. These manual rebalances incur costs.

Whereas in traditional finance as well as with centralised cryptocurrency exchanges users need to pay to rebalance their portfolio, with Hadouken the rebalancing is done for you - for no additional cost. Let's say you want to hold $100 of CKB and $100 of ETH. When the prices diverge, you might be holding $125 of CKB and $75 of ETH, or vice-versa. However, with a Hadouken liquidity pool, your stake in the pool's constituents will always be 50/50. If the price of CKB goes up relative to ETH, you will own slightly less CKB than you deposited, such that your stake in both coins is roughly equivalent in USD. And the best part is, as a liquidity provider you're _paid_ for these rebalances, rather than _paying_ for them !

Clearly this is a large improvement over user-assisted portfolio rebalancing, which will always cost something if done by oneself. During the 2021 bull run, a single swap on Ethereum at times costed more than $200!

## Impermanent Loss

For those unfamiliar with liquidity pools, you need to be familiar with a concept called impermanent loss (IL). There are two sides to every coin, and in some cases IL is your friend while in other cases it may cause you to lose out on gains otherwise realised through simply holding a pair of coins.

Due to the nature of liquidity pools and the mechanism through which they provide liquidity at all times - much unlike a centralised exchange, which is prone to order books drying up in times of large downward price movements - most non-stablecoin liquidity pools aim for a 50/50 balance of the tokens in the pool. As such, when users deposit tokens into a pool - again, at a 1:1 ratio in USD terms - they receive LP tokens. And when users wish to exit a pool, they burn their LP tokens and receive a pro rata share of the pool. If prices have diverged, users will receive more of the token that has declined in price relative to the other token. Overall, their USD value of withdrawn tokens may at times be lower than the USD value of the tokens had the user simply held spot for both assets.

However, on the aggregate, liquidity providers can expect to see a decrease in volatility of their holdings. Using [an example of DAI and ETH](https://twitter.com/guil\_lambert/status/1412608674380632067) deposited into a LP on UniSwap over a three-year period, volatility averaged between 40% and 55%, versus 25% to nearly 100% for a hold strategy, though LPs should assume they will receive a lower return due to IL. If you believe in both tokens and want to hold a balanced amount (in USD) of both tokens at all times, another benefit of holding LP tokens is that they're infinitely self-rebalancing. Rather than swapping token A for token B at arbitrary intervals (e.g. daily, weekly, monthly) and incurring swap fees, by holding an LP token you are holding shares in a pool that self-rebalances with every single trade. The rebalance "fees" are covered by traders using the LP, rather than the liquidity provider.

For a quantifiable amount of IL you can expect given a particular divergence in the price of two coins, you can use this [IL calculator](https://dailydefi.org/tools/impermanent-loss-calculator/). The chart below shows how price can impact the amount of IL that a liquidity provider will experience given a certain return (_x_) in the price of a token. For example, when a token increases 500%, the liquidity provider will incur an IL of approximately 25% versus having simply held the token.

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

For more information on impermanent loss, check out [the blog post](automated-portfolios.md#portfolio-theory) where the prior example came from.