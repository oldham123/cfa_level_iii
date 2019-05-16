---
sequence: 21
title: 'Reading 21: Currency Management - An Introduction'
section: 8
sectionTitle: 'Asset Allocation and Related Decisions in Portfolio Management'
layout: reading
---

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

- Forward transactions do not require market-to-market transactions before settlement
  - However, it may be desirable or regulatorily mandated to mark the position to market value
    - This is present value of any gain (loss) that would occur if the contract were closed early with an offsetting transaction
      - An offsetting transaction entails the opposite of whatever is required by the trade
      - For example, for an intial trade to deliver 100 EUR, the offsetting transaction is to buy 100 EUR, to settle on the same date

- An FX swap is unlike other swaps, involving two transactions:
  - First, a spot transaction is used to offset the existing forward
  - Secondly, a new forward is entered into

- Currency options are expressed in terms of two currencies, where a call on one is a put on the other
  - For example, consider a call to buy 100 at a price of ZAR/GBP 14.56
    - This is an option to buy (a call) 100 GBP at a price of 14.56 ZAR per GBP
    - It is also an option to sell (a put) 1,456 ZAR in return for 100 GBP

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
  - Therefore, an expected return for a portfolio invested in multiple foreign assets can be calculated using a weighted average of each individual calculated return

- Variance of a portfolio invested in foreign assets is influenced by variance in asset value, and variance in foreign currency value:
$$
\sigma^2_{R_\text{DC}} \approx w^2_{R_\text{FC}} \cdot \sigma^2_{R_\text{FC}} + w^2_{R_\text{FX}} \cdot \sigma^2_{R_\text{FX}} + 2 \cdot w_{R_\text{FC}} \cdot w_{R_\text{FX}} \cdot \sigma_{R_\text{FC}} \cdot \sigma_{R_\text{FX}} \cdot \rho_{(R_\text{FC}\text{, } R_\text{FX})}
$$
  - Note that if $R_\text{FC}$ is a risk-free return, then its variance, as well as its correlation with any other return is zero
  - This formula can be used for each foreign asset in the portfolio, with each value then inserted into the similar formula for standard deviation of the entire portfolio

## 21.B: Discuss strategic choices in currency management

## 21.C: Formulate an appropriate currency management program given financial market conditions and portfolio objectives and constraints

- There is no optimal strategy for currency management that is either empirically or academically supported
  - Arguments in favour of a passive approach include:
    - Hedging is costly in both time and money
    - Currency markets are *zero-sum* in the long run, in that appreciation in one place is a depreciation elsewhere
    - Eventually they revert to fair values
  - Arguments in favour of an active approach include:
    - Short run fluctuations can be significant, and present opportunities
    - Capital flow restrictions and monetary policy cause values to deviate from true fair values

- Management strategies include:
  - **Passive hedging** involves matching the currency exposure of a benchmark
  - **Discretionary hedging** involves allowing tactical deviations from benchmark currency exposure
  - **Active currency management** involves even larger deviations in currency exposure, with a goal of excess return, not risk reduction
  - **A currency overlay** is an outsourcing of currency management, where an overlay manager may treat currency as its own asset class, taking positions based on expectations to generate alpha
  - A decision on currency management should be recorded in the IPS, specifying, for example:
    - The amount of FX exposure to be hedged
    - Allowed deviations
    - Rebalancing frequency
    - Benchmarks used

- Strategic considerations in currency management include the following:
  - Currency is more volatile in the short run, whilst in the long run it is less important
  - Correlation between foreign asset value and value of the local currency of that foreign asset increases volatility
    - Negative correlation dampens volatility
  - Correlation can vary over time
  - The costs of a single hedging transaction can be small, but full hedging and repeated rebalancing can quickly become expensive
  - If hedging options expire out-of-the-money, then the premium is forfeit
  - The time periods to be hedged are often longer than the time horizons of available currency forwards, necessitating FX swaps
    - These FX swaps realise gains and losses, increasing cash flow volatility
  - Maintaining cash accounts in multiple currencies increases overhead costs

## 21.D: Compare active currency trading strategies based on economic fundamentals, technical analysis, carry-trade, and volatility trading

- The use of economic fundamentals is based on an assumption that prices revert to true values over time
  - Currency value increases are considered likely if:
    - They appear undervalued to a larger degree than others
    - Their true value has upward momentum
    - Higher interest rates are creating greater demand
    - Lower inflation is eroding purchasing power more slowly
    - The local market has lower risk associated with it

- The use of technical analysis assumes that past price movements can be a good indicator of future price movements
  - Since humans are likely to react to pricing signals in similar ways, certain patterns can be expected to persist
  - The true theoretical value is deemed unimportant by users of this approach
  - Typical patterns that are observed include:
    - Currencies that have been **overbought** or **oversold** are likely to reverse
    - The existence of **support levels** at prices which, for psychological reasons, investors are more willing to buy at
    - The existence of **resistance levels** at prices which there are more offers to buy at
    - Signs that prices are *pushing through* support or resistance levels

- A **carry trade** is an investment in higher interest rate currencies, financed by a lower interest rate currency
  - **Covered interest rate parity (CIRP)** holds that the difference between spot and forward currency rates is the difference in the period interest rates
    - Higher interest rates cause a currency to trade at a discount
    - If one country has a higher interest rate than another, then the currency with the higher interest rate will depreciate, and the other will appreciate
  - **Uncovered interest rate parity (UCIRP)** holds that the forward rate resulting from CIRP is an *unbiased estimator* of the future spot rate
    - However, the currency with the higher rate typically depreciates by less than predicted
    - A carry trade exploits this violation of UCIRP
  - Consider a current BRL/USD rate of 2.41, with respective interest rates at 6% and 1%
    - This implies a forward rate for BRL roughly 5% lower
    - To initiate a carry trade, an investor can borrow 100 USD at 1%, convert to 241 BRL and invest at 6%
    - The amount repayable would be 101 USD, whilst the amount generated by the BRL investment would be 255.46 BRL
    - If, due to a violation of UCIRP, BRL has not sufficiently depreciated against USD, this will be convertable into more USD than is due on the loan
  - Carry trades are usually profitable, but can yield significant losses in periods of volatility and financial distress

- Volatility trading is a strategy of profiting from volatility
  - **Delta** is the change of an option price with respect to the price of the underlying
  - **Vega** is the change of an option price with respect to the volatility of the underlying
  - **Delta-hedging** is the creation of a portfolio that is **delta-neutral** or has a delta of zero
    - Price fluctuations in the underlying have no impact, only changes in their volatility
    - For example, if volatility is expected to increase, an investor can enter a **long straddle** by purchasing an at-the-money call and put
      - If volatility is expected to increase, an investor can sell them
      - Since these options, when combined, are delta-neutral, they are effective a way of buying or selling volatilty
    - A **strangle** is cheaper to enter into, using out-of-the-money options to establish a *minimum* fluctuation required to create an intrinsic value


## 21.E: Describe how changes in factors underlying active trading strategies affect tactical trading decisions

- Each of the following events should then trigger an appropriate response:
  - Relative currency appreciation should lead to reducing a hedge or increasing a long position
  - If volatility is rising then investors should make use of a strangle or straddle
  - If market conditions are stable, then carry trades can be executed
  - Carry trades can be composites of trades in multiple currencies, with exposure tilted towards and away from individual currencies based on market expectations
  - Delta-neutral portfolios can be adjusted into having net positive or negative deltas if expectations indicate the corresponding movement in the underlying is likely

## 21.F: Describe how forward contracts and FX swaps are used to adjust hedge ratios

- Forward contracts have the following advantages:
  - More flexible than futures
  - Available in terms of almost any desired currency
  - Do not require margin, reducing the complexity of engaging in the trade, and the required cash flows
  - Significantly more liquid markets

- Hedges can be either **static** (held until expiration) or **dynamic** (continuously reblanced)
  - Consider a portfolio containing a foreign asset of a certain value to be hedged:
    - Sell an amount of currency equal to the current foreign asset price in the forward market for a given period
    - Two days before maturing of the forward buy the required currency to cover the initial short position
    - Sell another amount of currency equal to the new value of the foreign asset if it has changed
  - If the amount hedged is not adjusted between the initiation of the hedge and its expiration, then it is static
  - If the amount hedged is adjusted by changing the amount hedged with a given periodicity, then it is dynamic

- **Roll yield** is return accrued due to the convergence of the forward price to the spot price
  - Consider an investor entering a one month forward contract to sell 100 CHF for USD at 1.05, whilst the spot price is 1.04
    - 100 CHF can be bought for 104 USD at the initial spot price
    - It can then be delivered at contract expiration for 105 USD, with a profit of 1 USD
    - Shorting CHF generates a profit because the forward is at a premium
  - By increasing the value of trades with positive roll yield, and decreasing that of trades with negative roll yield, hedging costs can be offset

## 21.G: Describe trading strategies used to reduce hedging costs and modify the risk-return characteristics of a foreign-currency portfolio

- Hedging can be expensive, perfect hedging even more so
  - Costs rise further if an investor wants to eliminate downside risks whilst maintaining upside gain
  - The following are all potential hedging strategies, in decreasing order of hedging cost:
    - **Over-hedging** when depreciation is expected allows for potential gain if the expectation is correct
    - At-the-money put options eliminate downside risk only, but can be expensive and have no instrinsic value
    - Out-of-the-money put options are cheaper, but retain some downside risk, until the underlying price hits the strike price
    - A **collar** combines an out-of-the-money put (bought) and call (sold), with the call removing some upside potential and generating premium income, whilst the put removes some downside risk
    - A **put spread** involves the purchase of an out of the money put, and selling another put even further out of the money, providing a corridor of downside protection between the two strike prices
    - A **seagull spread** combines a put spread with selling a call, to generate premium income in return for limiting upside potential
  - Even more exotic options can create more complex strategies:
    - A **knock-in** option prevents a vanilla option from activating unless the underlying reaches a prespecified price
    - A **knock-out** option kills a vanilla option if the underlying hits a prespecified price
    - **Binary** or **digital** options have payoffs that do not vary with the price of the underlying

## 21.H: Describe the use of cross-hedges, macro-hedges, and minimum-variance-hedge ratios in portfolios exposed to multiple foreign currencies

- A **cross-hedge**is a hedge that is achieved using an instrument without perfect correlation to the hedged asset
  - Whilst the hedging is imperfect, it can ocasionally be more efficient than constructing a perfect hedge

- A **macro-hedge** is a form of cross-hedge that operates at a risk factor level instead of an asset level
  - Bond futures might be used to hedge interest rate risk, and volatility trading might be used to hedge against volatility
  - Derivatives contracts built on multiple currencies can modify the currency exposure of an entire portfolio
  - The hedging is not perfect, but may still be adequate whilst being significantly cheaper and simpler than perfect hedging

- The **minimum-variance hedge ratio** is a rigorous approach to determining the appropriate hedging ratio, using regression to minimise tracking error between the hedging instrument and the portfolio
  - The hedge ratio is the beta of this regression
  - Note that this correlation is not static, and as the relationship changes, the effectiveness of the hedge can too
  - This technique is important when engaged in cross-hedging

- **Basis risk** occurs when movements in the hedged asset and hedging instrument are not identical
  - A direct hedge typically has low basis risk
  - A cross-hedge can vary in basis risk
  - The use of an MVHR is likely to entail the highest basis risk, since it is exposed to the problems of changing correlations over time

## 21.I: Discuss challenges for managing emerging market currency exposures

- Emerging market currency trading involves the following potential problems:
  - Larger bid/ask spreads due to lower trading volume
  - Lower liquidity and higher transaction costs
  - Making markets between two emerging market currencies is especially difficult, and compounds most of these issues
  - Trading in these currencies entails non-normal return distributions, with a higher probability of extreme events
  - Correlation between emerging market currencies can approach 1 in financial crises, due to contagion
  - Higher yields leads to significant forward discounts, which means that negative roll yield occurs for anyone attempting to sell the currency
  - **Tail risk** is the higher than expected likelihood of negative events, caused by regular government intervention suppressing market forces until the intervention becomes insufficient, leading to negative spikes

- Due to restrictions on capital flows from countries attempting to manage their currency, regular forwards may not be settleable
  - **Non-deliverable forwards** deal with that by allowing for settlement in a developed market currency