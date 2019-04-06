# Reading 21: Currency Management - An Introduction

## 21.A: Analyse the effects of currency movements on portfolio risk and return

- Consider an example exchange rate: Sell spot 1,000 at CAD/USD 0.98
  - CAD is the **price currency**
  - USD is the **base currency**
  - This rate means that 1,000 USD is being offered for immediate sale, at a price of 0.98 CAD per USD
    - In reality this transaction would take two days to settle but this is often ignored, except in the case of an FX swap

- Consider this example rate: Buy 500 USD/CHF six months forward at 1.07
  - This rate means that USD is being offered to buy 500 CHF, at a price of 1.07 USD per CHF, with the trade intended to settle in six months

- Currency prices are usually expressed in terms of a **bid** and an **ask** price
  - The lowest figure is presented first, by convention
  - The difference between the two is the profit going to the dealer
  - Given a quote of 0.9790/0.9810 CAD/USD, this means the following:
    - One USD can be bought for 0.9810 CAD
    - One USD can be sold for 0.9790 CAD
  - Note that the dealer always receives more, or delivers less

- Transactions can be settled immediately (spots) or in the future (forwards)
  - Forwards can be expressed as a direct quote, or as an adjustment to the spot quote in terms of forward points
    - Forward points should be divided by $10^n$ where $n$ is the number of decimal places that the spot price is quoted to
    - They should then be added to the spot price

- Forward trnsactions do not require market-to-market transactions before settlement
  - However, it may be desirable or regulatorily mandated to mark the position to market value
    - This is present value of any gain (loss) that would occur if the contract were closed early with an offsetting transaction
      - An offsetting transaction entails the opposite of whatever is required by the trade
      - For example, for an intial trade to deliver 100 EUR, the offsetting transaction is to buy 100 EUR, to settle on the same date

- An FX swap is unlike other swaps, involving two transactions:
  - First,a spot transaction is used to offset the existing forward
  - Secondly, a new forward is entered into

- Currency options are expressed in terms of two currencies, where a call on one is a put on the other
  - For example, consider a call to buy 100 at a price of ZAR/GBP 14.56
    - This is an option to buy (a call) 100 GBP at a price of 14.56 ZAR per GBP
    - It is also an option to sell (a put) 1,456 ZAR in return for 1,000 GBP

- When considering the impact of currency on portfolios, the following terminology is important:
  - **Domestic currency** is the investor's currency
  - A **domestic asset** is an asset with a value denominated in the investor's currency
  - A **foreign currency** is any other currency, and a **foreign asset** is any asset denominated in a foreign currency
  - **Foreign currency return** is the return of a foreign asset, $R_\text{FC}$ expressed in its local currency
  - **Local currency return** is the percentage change in foreign currency value $R_\text{FX}$
  - **Domestic currency return** is the return of a foreign asset expressed in domestic currency $R_\text{DC}$, accounting for both $R_\text{FC}$ and $R_\text{FX}$

- Any investment in a foreign asset is exposed to:
  - Risk of the asset
  - Risk of the asset's local currency
  - Hence, $R_\text{DC} = (1 + R_\text{FC}) \cdot (1 + R_\text{FX}) - 1$
    - $R_\text{FX}$ is calculated from two exchange rates, $R_0$ and $R_T$ using the following:
      - $R_\text{FX} = \frac{R_0}{R_T}$
      - Note that the two rates $R_0$ and $R_T$ should be expressed with the foreign currency as the base currency

- Variance of a portfolio invested in foreign assets is influence by variance in asset value, and variance in foreign currency value:
$$
\sigma^2_{R_\text{DC}} \approx w^2_{R_\text{FC}} \cdot \sigma^2_{R_\text{FC}} + w^2_{R_\text{FX}} \cdot \sigma^2_{R_\text{FX}} + 2 \cdot w_{R_\text{FC}} \cdot w_{R_\text{FX}} \cdot \sigma_{R_\text{FC}} \cdot \sigma_{R_\text{FX}} \cdot \rho_{(R_\text{FC}\text{, } R_\text{FX})}
$$
  - Note that if $R_\text{FC}$ is a risk-free return, then its variance, as well as its correlation with any other return is zero