# Borrow and Lend

Using Hadouken, users can borrow against - and lend out - various cryptocurrencies including CKB, WBTC, ETH, and BNB, with more to come in the future.

Starting with deposits, users can earn yield on their assets by depositing them into Hadouken Lend, which is built on top of Aave and shares the same mechanics. Like Aave’s aTokens, Hadouken has hTokens, which represent user deposits onto the platform. Based on the amount of deposited tokens being loaned out at any given time, the deposit rate will vary. Every block, depositors share the interests paid by borrowers corresponding to the average borrow rate multiplied by the utilisation rate.

On the other side naturally is borrowing. Often times, an investor might want to unlock liquidity from some of their assets without selling, for example, because they think the asset will still appreciate in value and they don't want to dispose of it and incur a taxable event in the process. On the flip side, they might want to borrow an asset to sell it, creating a synthetic short position without the need for a centralised exchange. Using Hadouken Lend, users can borrow against their assets with either stable or variable rates.

Depending on the collateral asset, a user can typically borrow about 30% of the posted collateral. They are then assigned a health factor, which represents the safety of a user's deposited assets against the borrowed assets and their underlying value. As the value of the collateral changes, the health factor changes. A higher health factor is better, and a lower health factor puts the borrower at risk of liquidation, which occurs when the health factor reaches 1. If the health factor approaches 1, the borrower can either repay part or all of the loan, or post more collateral against the loan to avoid liquidation.

[_**For more information, please refer to Aave's docs**_](https://docs.aave.com/faq/borrowing).