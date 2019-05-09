---
sequence: 28
title: 'Reading 28: Active Equity Investing'
section: 10
sectionTitle: 'Equity Portfolio Management'
layout: reading
---

# Reading 28: Active Equity Investing

## 28.A: Compare fundamental and quantitative approaches to active management

- Active management comes in two main forms:
  - **Fundamental active management**
    - These approaches mostly rely on the judgement of a skilled analyst
    - Analysts combine research on company fundamentals with their experience and judgement to estimate intrinsic values
    - Compared to a quantitative approach, there will be fewer positions, each with larger allocations
      - Losses can occur if:
        - The analyst is incorrect in their valuation
        - The mispricing fails to be recognised by the market and therefore doesn't correct
  - **Quantitative active management**
    - These approaches rely on models built upon rules that generate recommendations
    - Statistical expertise and large amounts of data are required
    - Analysts seek to uncover relationships between risk factors and returns across a large set of stocks
    - Optimisation methods determine asset allocations that maximise alpha
    - The portfolio is rebalanced with a predetermined frequency
  - Note that it is the way in which the final investment decision is made that determines what form of strategy is being used

## 28.B: Analyse bottom-up active strategies, including their rationale and associated processes

## 28.C: Analyse top-down active strategies, including their rationale and associated processes

- Bottom-up strategies mostly utilise data on individual firms, such as profitability
  - A bottom-up manager blending top-down methods might include a top-down derivatives overlay to adjust exposure to macro risk factors
  - A quantitative bottom-up manager will attempt to identify relationships between firm fundamentals and expected return
  - A fundamentals bottom-up manager will include qualitative information on items such as management, and branding
  - Value-based approaches include:
    - Relative-value methods, comparing price multiples between firms
    - Contrarian investing
    - High-quality investing, seeking value stocks with evidence of underlying financial strength
    - Deep-value investing, searching for opportunities amongst very cheap stocks, such as firms undergoing financial troubles
    - Distressed debt investing, purchasing stocks in firms shortly before liquidation
  - Growth-based approaches include:
    - Momentum investing, seeking firms with recent strong results
    - "Growth at a reasonable price" investing

- Top-down strategies mostly utilise data on macro variables
  - A top-down manager blending bottom-up methods might use bottom-up analysis to identify high quality individual securities consistent with the desired factor exposure
  - Managers make use of ETFs and derivatives to adjust exposure to various risk factors such as:
    - Geography
    - Sector
    - Volatility
    - Thematic strategies, such as regulatory change, the shift to cloud computing, or renewable energy

## 28.D: Analyse factor-based active strategies, including their rationales and associated processes

- A **factor**is some variable that is correlated with portfolio returns
  - Factors postiviely correlated with returns are *rewarded factors*
  - Factors negatively correlated with returns are *unrewarded factors*
  - Aggressive backtesting can identify spurious factors, so a relationship must be supported not only by data, but by a sound economic rationale

- The **Hedged Portfolio Approach** functions in the following way:
  - Establish the set of investable stocks
  - Rank the stocks according to some factor, with the order of the ranking determined by whether it is *rewarding* or *unrewarding*
  - Divide the stocks into quantiles according to this ranking
  - Go long the best quantile, and short the worst quantile
  - Disdvantages include:
    - Information contained within the middle quantiles is neglected
    - Linear relationships between returns and factors are assumed
    - These portfolios can give the appearance of diversification, but may not be if factors are correlated
    - The ability to short sell is assumed
    - The portfolio will typically necessitate exposure to multiple other factors as well
      - A portfolio with exposure exclusively to one desired factor is called a **factor mimicking portfolio**
      - They can be difficult to construct, with the necessary liquidity and short sellability often lacking

- A specific variant of factor-based investing is **equity style rotation**
  - This strategy is predicated on the notion that various factors are most postively correlated at different times
  - This means that the ideal factor exposure changes will change

## 28.E: Analyse activist strategies, including their rationale and associated processes

- **Activist investing** involves seeking a sufficient stake in order to holding significant voting influence, and than agitating for changes that enhance stock value
  - The process typically involves:
    - Establishing a set of investment opportunities
    - Buying an initial stake
    - Submitting suggested changes, perhaps via open letter
    - Threaten a *proxy contest*
    - If necessary, initiating a proxy contest
  - Activist investing first began in the 1970s, but has recently become significantly more common

- Tactics used by activists include:
  - Seeking board representation
  - Writing open letters
  - Proposing changes at a shareholder AGM
  - Proposing restructuring that transfers wealth to shareholders
  - Reducing compensation
  - Initiating legal challenges as a response to possible breaches of fiduciary duty
  - Campaigning publicly against management
  - Breaking up inefficient conglomerates

- Defenses against activist investing include:
  - Multi-class share structures, entitling privileged voting rights to specific shareholders
  - "Poison pill" provisions
  - Staggered board elections, preventing wholesale replacement of the entire board

- The targets of activist investing tend to be firms that are performing badly, despite a latent potential for growth and strong earnings
  - For example, a firm that owns valuable IP but is failing to use it effectively

- Empirically, activist investing can trigger growth and profitability
  - However, it additionally can lead to increased debt levels
  - Additionally, other investors tend to react positively upon the announcement of activist behaviour, with stock prices more likely to rise afterwards

## 28.F: Describe active strategies based on statistical arbitrage and market microstructure

- **Statistical arbitrage** is a strategy of exploiting pricing inefficiency
  - **Pairs trading** involves identifying two highly correlated securities, seeking to profit from mean reversion following a temporary divergence
  - **Market microstructure-based** strategies try to take advantage of mismatches between supply and demand that last for milliseconds
  - **Event-driven** strategies seek to identify mispricing in the immediate aftermath of events such as M&A activity
    - A manager can buy stocks in a target firm upon announcement, whilst there is still uncertainty due to regulatory approval that delays a price rise

## 28.G: Describe how fundamental active investment strategies are created

- The fundamental active investment process usually proceeds as follows:
  - Define a set of investible securities
  - Prescreen the total set until the remaining number is manageable, according to some broad criteria
  - Investigate the industry, competitive environment, and other factors
  - Forecast performance using firm fundamentals
  - Derive valuations
  - Construct a portfolio using these valuations, according to presepcified risk constraints
  - Rebalance as needed

- Issues with fundamental investing include:
  - Behavioural biases
  - **Value traps**, where a price drop makes a stock appear attractive, in turn leading to overvaluation, only for the price to continue falling, since the reason the price is low is due to weak fundamentals
  - **Growth traps**, where growth prospects have already been priced in, possibly to an excessive degree

## 28.H: Describe how quantitative active investment strategies are created

- Quantitative investing follows a clear procedure
  - Opportunity definition
  - Data acquisition
    - Large datasets are required to provide reliable conclusions
    - Collecting, arranging, and cleaning the data is often necessary
    - Data required often includes:
      - *Company mapping*, tracking the history of firms as they combine and split over time
      - *Company fundamentals*
      - *Survey data*
      - *Unconventional datasets*
  - Back-test identified relationships
    - Once strategies are identified, they can be applied to historical data to determine their performance
    - Correlation between factor exposure and returns can indicate performance
      - If the relationship is strong then the factor is said to have "high predictive power"
    - Conduction of backtesting could proceed as follows:
      - Obtain historical data on a cross section of firms
      - Calculate values for the relevant factor
      - Rank stocks by the factor exposure, i.e. the number of standard deviations the firm is away from the average value
      - If the relationship between the factor and returns is linear, then the **Pearson information coefficient** is the correlation between factor exposure and returns
      - Since Pearson IC is sensitive to outliers, the **Spearman Rank IC** is also used
        - Spearman Rank IC is the IC of the rank of the factor scores and the rank of performance
  - Evaluate results and likely returns
    - Out-of-sample testing evaluates the model according to datasets that weren't involved in its construction
  - Portfolio construction
    - This is done with the assistance of risk models, used to calculate return volatility according to the volatility of each position, as well as pairwise correlations

- Issues with quantitative investing include:
  - Survivorship bias, due to back-tests only being run against firms which lasted throughout the entire historical period used
  - Look-ahead bias, resulting from a model assuming that information was available to assist decisions at a time when it likely wasn't
  - Data-mining, resulting from an aggressive search for a historical data set which validates a model
  - **Quant overcrowding**, resulting from a popular strategy being abandoned by many managers simultaneously due to poor performance

## 28.I: Discuss equity investment style classifications

- Investment style classification aims to arrange stocks into broad groups, where correlation within is high, but correlation without is low
  - There are two main approaches:
    - **Holdings-based**
      - This approach analyses attributes of individual stocks in a portfolio
      - These are aggregated to determine the style of the portfolio as a whole
      - The approach may aim to place a similar number of stocks into each category, along two dimensions
        - Consider for example, classification as either *value* or *growth*
        - A stock can be assigned a *style score* between one and one hundred, determining to what degree a stock is value, and to what degree it is growth
        - The difference of these is a *net style score*, used to classify
      - Holdings-based analysis is difficult to perform if a derivatives overlay is used, unless there is good information available about the strategy being followed
    - **Returns-based**
      - By regressing fund returns against a collection of indices, each thought to strongly represent investment of a certain style
      - The degree to which a fund's returns are correlated with the returns of an index, the fund can be thought of as being of that style
  - Additionally, a fund manager will often self-identify a fund's style
    - This self-identification can be compared to the results of both approaches, perhaps identifying a need for further investigation if results are inconsistent