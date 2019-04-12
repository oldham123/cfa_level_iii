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