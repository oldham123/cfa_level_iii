---
sequence: 27
title: 'Reading 27: Passive Equity Investing'
section: 10
sectionTitle: 'Equity Portfolio Management'
layout: reading
---

# Reading 27: Passive Equity Investing

## 27.A: Discuss considerations in choosing a benchmark for a passively managed equity portfolio

- A benchmark index should be:
  - **Rules-based**: Stock inclusion/exclusion, weighting, and reblancing decisions must be based on consistent rules to allow replication
  - **Transparent**: The rules should be public and clear
  - **Investable**: The included assets must be such that replication is possible

- In selecting a benchmark, the desired exposure must be determined
  - The following can be considered as guides to this determination:
    - *Market segment*, including choices of industry, geography, and developed, emerging, or frontier markets
    - *Capitalisation*, small, mid, and large cap stocks provide different exposures
    - *Growth versus value*, where growth stocks have higher P/B and P/E ratios
    - Other risk factors include momentum, liquidity, and volatility

- An index can be constructed in multiple ways
  - An **exhaustive** index includes every stock within a given market
  - A **selective** index will only include a subset

- Weighting methods can also differ
  - *Market-cap weighting*
    - This method also closely mimics *liquidity weighting*
    - One common method uses capitalisations that exclude closely held shares
  - *Price weighting*
    - This is similar to holding an equal number of shares of each firm, and is uncommon
  - *Equal weighting*
    - Relative to market-cap weighting, small-cap stocks have higher representation using this method, and the index is therefore more volatile
    - This method requires frequent rebalancing
  - *Fundamental weighting*
    - Based on the premise that stock prices are ultimately determined by fundamental factors such as sales or earnings

- **Stock concentration** can be captured using the **Herfindahl-Hirschman index (HHI)**, which expresses concentration in terms of an *effective number of stocks* in an equivalent, equally weighted portfolio
  - A market-cap weighted index invested in 100 firms, may have an effective number of stocks of only 20, due to the high weighting of large-cap stocks
  - Effective number of stocks is the reciprocal of the HHI, where  $w_i$ is the weighting and is given by:
$$
\text{effective number of stocks} = \frac{1}{\sum^n_{i = 1} w^2_i}
$$

- The stocks included in an index change over time, usually as part of two processes:
  - **Rebalancing** is the process of adjusting composition of the index to the desired weights following the distorting effects of price changes
  - **Reconstitution** involves removing stocks that are no longer appropriate for the index's desired risk exposure
  - There can be pricing effects as stocks are included and excluded, which can be exploited through arbitrage, if an investor can predict when stocks are likely to be included or excluded

## 27.B: Compare passive factor-based strategies to market-capitalisation-weighted indexing

- Replication of a benchmark index can be done by either:
  - Investing in all, or a subset of, the same stocks as the index, or
  - By creating a portfolio with the same exposures to risk factors, in a strategy called **passive factor-based investing**, or **smart beta**
  - These risk factors include:
    - *Growth factor*, exposure to firms with high P/B or P/E ratios
    - *Value factor*, exposure to firms with low P/B or P/E ratios
    - *Size factor*, exposure to firms with low market capitalisation
    - *Yield factor*, exposure to high-dividend stocks
    - *Momentum factor*, exposure to stocks with strong recent returns
    - *Quality factor*, exposure to consistently well-performing firms
    - *Volatility factor*, exposure to low risk stocks
  - The ability to mimic factor exposure can vary

- Passive factor-based strategies can be:
  - *Return-oriented*, focusing on dividends, momentum, and fundamentals
  - *Risk-oriented*, focusing on volatility
  - *Diversification-oriented*, focusing on maximising diversification benefits

## 27.C: Compare different approaches to passive equity investing

- There are three common approaches to passive equity investing:
  - **Pooled investments**
    - Open-ended mutual funds and exchange traded funds are examples of this
    - Costs are low, and the fund structure provides convenience for the participating investors
    - ETFs can usually provide shareholder redemption more cheaply than open-ended mutual funds, through delivery of actual shares, reducing taxable gains and losses
    - ETFs also suffer from higher transaction costs (due to commissions) and illiquidity in some secondary ETF markets
  - **Derivatives-based strategies**
    - Derivatives can be added to portfolios as an *overlay* to adjust overall risk and return characteristics
      - *Completion overlays* restore risk exposure to that of a benchmark
      - *Rebalancing overlays* restore the constitution of the portfolio to match the benchmark
      - *Currency overlays* can increase or reduce currency risk
    - The use of derivatives to adjust exposure is often faster and cheaper, and more liquid
    - Derivative contracts expire however, and must be rolled over in order to maintain one's position
    - Exchange-traded derivatives may not meet specialty requirements, and OTC derivatives introduce counterparty risk

## 27.D: Compare the full replication, stratified sampling, and optimisation approaches for the construction of passively managed equity portfolios

- **Full replication** involves tracking a benchmark index by holding the same securities in the same proportions as the index
  - This can be costly, especially for large indexes, with some stocks having low liquidity
  - Full replication requires regular rebalancing and reconstitution
  - This method allows for close matching of index return (before costs)

- **Stratified sampling** involves selecting a subset of the stocks included in a benchmark index
  - A manager divides the stocks within an index into various **strata** across multiple dimensions:
    - Industry
    - Style
    - Geography
    - Size
  - The manager then selects stocks from each strata so as to reduce tracking error
    - The cheapest and most liquid stocks are selected first
  - The more dimensions used, the smaller the tracking error

- **Optimsation** makes use of modern portfolio theory to construct a portfolio of a subset of stocks from the index that would have minimised tracking error
  - The process can have constraints applied to it, and can be combined with stratified sampling
  - This process involves what could be construed as an over-reliance on historical relationships that may not continue to hold

## 27.E: Discuss potential causes of tracking error and methods to control tracking error for passively managed equity portfolios

- Tracking error is the difference between portfolio return and benchmark return
  - As the sample size increases and more stocks are added to a portfolio, tracking error decreases
  - However, as managers run out of more liquid stocks to select, tracking error starts to increase due to higher transaction costs
  - Furthermore, the more rebalancing and reconstitution that is required, the more cash must be paid for trade execution
  - Higher cash requirements, such as needed to meet redemptions, create **cash drag**, since cash is the lowest return asset
  - An equity index is designed to represent theoretical pure investment in equities, whereas actual passive equity portfolios will always have some level of cash requirements, for example, to cover transaction costs
  - In general, there are trade-offs between more accurate replication, and transaction costs

## 27.F: Explain sources of return and risk to a passively managed equity portfolio

- **Attribution analysis** is the act of determining the sources of return within an index
  - If these sources are well understood, then the index can be more efficiently replicated

- **Securities lending** can be used to offset transaction costs and reduce tracking error

- **Investor activism** and **corporate engagement** can be used to enhance returns, and is a key component of active management
  - Passive investors can't simply sell shares in firms with bad management, so activism and engagement can be valuable to them too
  - Additionally, all managers have a fiduciary duty to take the steps necessary to invest in the best interests of their clients
  - However, proxy voting in an informed manner can involve costly research, and many managers make use of proxy voting services