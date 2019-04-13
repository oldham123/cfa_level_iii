# Reading 23: Liability-Driven and Index-Based strategies

## 23.A: Describe liability-driven investing

- When a portfolio exists in order to meet a definable future liability, **liability-driven investing** may be used
  - **Asset-liability management** is the use of strategies focused on the overall surplus or deficit between portfolio assets and liabilities
    - If the present value of liabilities and assets both change with variable rates then this approach may be appropriate
  - **Liability-driven investing** accepts the existence of future liabilities as a given and manages assets in order to cover those liabilities
  - **Asset-driven investing** accepts the existence of current assets as a given and manages future liabilities with respect to those assets

- LDI is usually more applicable to institutional investors, but it can be useful for individuals too, for example if they have a future goal that they want to be able to meet
  - There are four main types of liability
    - **Type I liabilities** have known amounts and payment dates
    - **Type II liabilities** have known amounts but uncertain payment dates
    - **Type III liabilities** have uncertain amounts but known payment dates
    - **Type IV liabilities** have uncertain amounts and payment dates
  - Whilst simple duration is appropriate for modelling liabilities of type I, modified duration is required for the other three

## 23.B: Evaluate strategies for managing a single liability

- **Immunisation** is the minimisation of return variability over a given time period
  - This allows for reliable calculation of the future value of plan assets, and assurance that a future liability can be met
  - The goal of an immunised portfolio is to earn its initial IRR, in order to grow to a future value sufficient to fund the liability
  - **Cash-flow matching** is a simple form of immunisation, which involves purchased a fixed-income instrument that provides inflows identical to the outflows associated with a liability
    - **Macaulay duration** is the weighted-average time until cash flows due from an asset are received
      - Since all the cash flows of a zero-coupon bond are received at maturity, macaulay duration of a zero coupon bond is also maturity
      - Non-zero-coupon bonds have coupon payments that cause the macaulay duration to be less than maturity
      - A cash-flow matched portfolio will have the same macaulay duration as the liabilities it aims to fund
        - **Price risk** is the risk to returns if the bond must be sold before maturity
        - **Reinvestment risk** is the risk to returns due to the uncertain returns on reinvested cash flows
        - Macaulay duration is a point at which these risks offset each other
    - **Modified duration** is the macaulay duration divided by the periodic discount rate used in calculating the present values of cash flows
      - Modifed duration is slightly more suited to measuring price change of an asset
      - Macaulay duration is slightly more suited as a measure of time for immunisation purposes

- Rather than computing values based on weighted averages of the assets within the portfolio, **portfolio statistics** can be used
  - Portfolio statistics are directly calculated from portfolio cash flows
  - With a flat yield curve using portfolio statistics instead will not yield any differences, but they will if the yield curve slopes upward
  - Whilst portfolio statistics are generally more appropriate, weighted average values can be used, but they can introduce errors into the approximation

- **Dispersion** refers to the dispersion of cash flows from fixed income assets
  - Dispersion has a non-negligible impact on the success of immunisation strategies due to convexity
$$
\text{convexity} = \frac{\text{Macaulay duration}^2 + \text{Macaulay duration} + \text{dispersion}}{(1 + \text{periodic IRR})^2}
$$
  - Consider an investor with a liability due in five years, with a portfolio they intend to use to immunise it
    - The portfolio is composed of twofixed income assets, one with longer, and one with shorter duration than the liability
    - Overall portfolio duration matches that of the liability, and the present values of both are equal
    - Additionally, portfolio convexity exceeds that of the liability
      - Higher convexity leads to a smaller price shift for a given change in yields, ensuring that the portfolio will exceed the amount required by the liability
    - This scenario demonstrates that using duration matching instead of cash-flow matching preserves some structural risk
      - Assets and liabilities that are matched only on durations but not cash flows can perform differently under the same yield curve shifts
      - Since most shifts are parallel, this structural risk usually benefits the investor
    - This also demonstrates why immunisation is also referred to as **zero-replication**
      - As the yield curve shifts, the resulting changes in the present values of the assets and liabilities either perform as well as or better than a zero-coupon perfectly matched to the liability
        - It is important to note that none parallel shifts that don't result in this positive outcome are possible, i.e. the strategy is not risk-free
        - Additionally, the duration of the portfolio is not fixed, and so rebalancing will be required
    - If the yield for the lower duration asset falls, whilst that of the higher duration increases (i.e. a *steepening twist*) the value of the longer duration bond will decrease by more than the increase for the shorter duration bond
      - However, the likely increase in IRR may still allow the portfolio to fund the liablility
      - In the opposite case (i.e. a *flattening twist*), the increase in value of the longer duration asset may exceed the fall of the shorter duration asset
        - However, IRR is likely to decrease, which must also be considered
    - In a *positive butterly twist* the yields of both assets rise, whilst the liability yield falls
      - This is likely to lead to a significant chance of not being able to fund the liability due to a fall in value of the portfolio, and an increase in the present value of the liability
        - IRR may increase but this yield curve movement may create significant structural risk
    - In the inverse scenario, a *negative butterfly twist*, the values of the portfolio and liability are highly likely to shift favourable, but there is significant risk of a fall in portfolio IRR relative to the liability discount rate
  - Overall, risk is reduced by reducing dispersion of asset cash flows around those of the liability
    - This reduces convexity, and risks associated with yield curve shifts

## 23.C: Compare strategies for a single liability and for multiple liabilities, including alternative means of implementation

- **Cash flow matching** is the lowest risk immunisation strategy
  - Risks are so low that it may allow *accounting defeasance*, where liabilities are removed from the balance sheet entirely, along with the assets dedicated to funding them
  - Zero-coupon bonds are the simplest instruments to achieve cash flow matching, but it can also be done with coupon bearing bonds
    - The precise coupon bearing bonds required for cash flow matching are unlikely to be available
    - A *cash in advance* constraint requires assets used to fund liabilities to pay out slightly before those liabilities are due, but this can create reinvestment risk

- **Duration matching** is a more flexible approach, where asset and liability macaulay durations must match
  - Matching **money duration** however is a more common methodology, featuring the following steps:
    1. Ensure that $\text{PV(assets)}>\text{PV(liabilities)}$
    2. Ensure that $\text{BPV}_\text{assets} = \text{BPV}_\text{liabilities}$
      - $\text{BPV} = \text{modified duration} \cdot \text{value} \cdot 0.0001$
    3. Ensure that dispersion and convexity of assets slightly exceeds that of liabilities
    4. Rebalance the portfolio regularly to maintain $\text{BPV}$ matching

- The costs of adjusting portfolio assets can be avoided through the use of a **derivatives overlay**
  - Futures contracts can be included into a portfolio to adjust its duration
  - In the US, such contracts are available based on the 30 year bond, and the two, five, and ten year Treasury notes
  - The seller of these contracts must provide $100,000 par of a deliverable security
  - In return the buyer pays the price of the contract, multiplied by some conversion factor $\text{CF}_\text{CTD}$
  - The bond that the seller chooses to use to satisfy the terms of the contract determines the duration of the contract
$$
\text{BPV}_\text{future} \approx \frac{\text{BPV}_\text{CTD}}{\text{CF}_\text{CTD}}
$$
  - This can be used to determine the number of futures contract should be added to a portfolio in order to restore duration matching
$$
N_f = \frac{\text{BPV}_\text{liability} - \text{BPV}_\text{portfolio}}{\text{BPV}_\text{futures}}
$$

- **Contingent immunisation** combines an active and passive outlook
  - Provided that the portfolio has a sufficient surplus, active management can be used with a goal of generating alpha
  - If the surplus shrinks, the portfolio should be immunised before it reaches zero
  - Some CI approaches can create liquidity risk, particularly if the entire portfolio is being actively managed (instead of just the surplus)
    - Rapid immunisation would require rapid liquidation of assets

## 23.D: Evaluate liability-based strategies under various interest rate scenarios and select a strategy to achieve a portfolio's objectives

- Recall how duration effects the relationship between a change in yields and a change in prices
$$
\Delta \text{PV}=(-\text{modifed duration} \cdot \Delta Y)+(\frac{C}{2} \cdot \Delta Y^2)
$$
  - Keeping everything else fixed, for a given increase in interest rates, higher duration means a larger fall in prices, and vice versa
  - If an increase in interest rates is expected, instead of duration matching, it may be desirable to ensure that asset value falls by less than that of liabilities
  - This can be done by underhedging, or buying fewer futures contracts, so that asset duration is lower than liability duration
  - If rates are expected to fall, overhedging can be used

- The use of a derivatives overlay creates additional risks
  - There is a requirement to post margin daily
  - Interest rate swaps may be an alternative that avoid this requirement
    - Purchasing a receive-fixed swap is equivalent to purchasing a bond, and reduces duration
    - Purchasing a pay-fixed swap increases duration
    - The lack of a requirement to post daily margin is not necessarily the case everywhere, or permanently the case
      - In some cases regular marking to market is required

- A **swaption** is the right to enter a swap, purchased by paying an initial premium
  - To increase portfolio duration, an investor could purchase a receiver swaption
    - The investor now has the right to initiative a receive-fixed swap at a predetermined **swap fixed rate (SFR)**
    - To establish whether a swap has value, its SFR can be combined to the SFR of new swaptions
    - If the new SFR is lower, then the right to receive fixed adds value to the portfolio
    - Otherwise, the swaption expires worthless
      - Note that entering a swap would have entailed losses
  - Investors can also combine swaptions into a **swaption collar**
    - This technique reduces the cost of a receive-fixed swaption by selling a pay-fixed swaption
      - This however reduces the upside of an increase in rates, as the investor would have to pay variable in return for fixed if the swaption is activated

## 23.E: Explain risks associated with managing a portfolio against a liability structure

- Managing a portfolio with the express purpose of funding liabilities has a series of risks associated with it:
  - The calculated hedge amounts are, ultimately, approximations, and many calculations neglect convexity
    - Convexity must be accounted for if the yield curve shifts are significant
  - Duration calculations assume that the yield curve shifts in a parallel fashion
  - A twisting yield curve can nullify the ability of an immunisation strategy to replicate a zero-coupon bond
    - Portfolio convexity relative to liabilities should be slightly increased whilst minimising dispersion
  - Measurement errors can accumulate if portfolio statistics are neglected in favour of weighted averages of assets
  - The CTD of a futures contract can change, whilst many calculations assume it does not
  - The use of OTC derivatives as part of a derivative overlay exposes the investor to counterparty risk

## 23.F: Discuss bond indices and the challanges of managing a fixed income portfolio to mimic the characteristics of a bond index

- Bond indices providing a range of exposure options exist
  - Investing in an index is an alternative to management of fixed income assets, providing a similar diversification benefit
  - The aim of such an index is to minimise **tracking error**
    - Tracking error is the standard deviation of active return
  - The **pure index**, or **full replication** methodology involves holding the same assets with the same weights as the index
  - **Enhanced indexing** aims to replicate the same risk exposures but using different assets, since actual full replication can entail significant transaction costs

- Fixed income indexing presents several challenges:
  - The market is larger and more varied than the equities market
  - Each issue from a single issuer is likely to vary greatly in liquidity
  - Capital requirements have increased, leading to larger dealer spreads, and reduced liquidity
  - Transactions for a specific issue may be rare, and are likely to be private, leading to a lack of reliable data
    - Bond prices can be implied through matrix pricing, but this is not a perfect technique
  - The composition of a fixed income index can undergo significant changes rapidly as issues mature, and new bonds are issued

- As an alternative to full replication, an investor may attempt to match the following:
  - Modified duration, in order to reduce tracking error due to parallel yield curve shifts
    - The presence of embedded options necessitates the use of **effective duration**
  - Matching durations at specific *key rates* can reduce tracking error from non-parallel yield curve shifts
  - Match exposures to various sectors, and credit qualities
  - Another technique is to match the present value distribution of cash flows

- **Stratified sampling** is a technique used to implement enhanced indexing
  - Identify the main attributes of the index to match (e.g. credit quality, sector, maturity)
  - Determine the weights of each present in the index
  - Choose assets that replicate these weights

## 23.G: Compare alternative methods for establishing bond market exposure passively

- Indirect exposure provides the diversification benefits of fixed income investing without directly investing in bonds
  - This can be done using funds, or derivates
  - Whilst some costs of fixed income investing are avoided, these approaches can incur costs and risks of their own

- **Mutal funds** with a focus on the fixed income market may be appropriate for smaller, or individual investors
  - By leveraging large amounts of aggregated capital they may be able to benefit from tighter spreads in OTC trades
  - Shares in **open-ended** funds can be bought or sold with respect to the fund's **net asset value (NAV)**
    - Participation in these funds can entail transactional costs
    - Shares in these funds, unlike bonds, do not mature, and the income stream from them can change over time
    - They can only be bought or sold once per day

- **Exchange traded funds** trade shares continuously on exchanges
  - **Authorised participants** can sell shares in the fund and receive a share of the fund assets
  - They can also sell a package of underlying assets to the fund in return for an increased share
  - Whilst this leads to arbitrage between shares in the fund and the NAV, it isn't a very effective process due to the illiquidity of underlying assets

- **Synthetic strategies** make use of derivatives in order to obtain passive exposure
  - A **total return swap** involves an investor agreeing to paying LIBOR plus some rate, in return for receiving the rate of return on a fixed income index
    - Unless collateralised, this is effectively the same as a leveraged investment in the index
    - The counterparty to such a transaction is in general a dealer who can replicate the index more efficiently than an individual investor
    - Disadvantages of this strategy include:
      - The underlying assets are not owned
      - The term is normally shorter, and introduces rollover risk
      - If the point of the transaction is to gain exposure where it would otherwise be difficult (e.g. due to illiquidity), this will be reflected in the spread paid
      - Regulatory changes are increasing costs and requirements on dealers, making these transactions more costly in turn for investors
  - **Exchange traded derivatives** are another alternative, although regulatory changes are affecting them also
    - Futures contracts that provide exposure to bond indices have been available since 2006 but their popularity, and thus availability, has waned

## 23.H: Discuss criteria for selecting a benchmark and justify the selection of a benchmark

- Selection of bond indices has several complications:
  - Duration declines over time for a static fixed income portfolio
  - Index composition may undergo dramatic shifts due to issue maturation, or new issuance
  - A value-weighted index may overweight issuers with lower creditworthiness, since they issue more bonds

- One way of constructing fixed income portfolios is the use of **smart beta rules**
  - This is a methodology that involves establishing simple rules that can be followed to add value
    - One example is to determine desired exposures to various sectors, as well as desired duration, leading to a *custom index*
    - Another is a **credit barbell**, with longer term US treasuries used to increase duration, with shorter term corporate bonds used to increase return

## 23.I: Describe construction, benefits, limitations, and risk-return characteristics of a laddered bond portfolio

- A **laddered portfolio** features roughly equal par amounts of fixed income securities maturing each year
  - This portfolio has identical duration to both a bullet portfolio and a barbell portfolio, but with other key differences
    - A laddered portfolio has higher liquidity due to bonds maturing each year
    - A laddered portfolio achieves greater diversification across maturities
    - This portfolio protects against reinvestment risk because naturally some cash will be reinvested at higher rates, and some at lower rates
    - A laddered portfolio has higher convexity than a bullet portfolio, which can generate returns in the event of a parallel yield curve shift
  - Instead of a laddered portfolio of bonds, one can be constructed from **target date** bond ETFs
    - Each will mature in a designated year, passively managed to replicate a bond maturing
    - This can reduce management costs compared to actual fixed income investing