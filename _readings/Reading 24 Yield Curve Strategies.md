---
sequence: 24
title: 'Reading 24: Yield Curve Strategies'
section: 9
sectionTitle: 'Fixed Income Portfolio Management'
layout: reading
---

# Reading 24: Yield Curve Strategies

## 24.A: Describe major types of yield curve strategies

- A yield curve is an illustration of the relationship between **yield** and **maturity**
  - The *yield* could mean:
    - **Yield to maturity** (most common)
    - Spot rates
    - Forward rates
  - The yield curve is not static, and changes over time
    - It can shift upwards or downwards
    - It can become flatter or steeper
    - It can become more or less curved
  - The appropriate strategy to employ depends on the type of shift that a manager expects

- Strategies that might be used include:
  - **Buy and hold**
    - If the curve slopes upward, increasing maturity and duration allows an investor to earn a higher yield
    - Turnover will be low, and hence so will transaction costs
    - Active management may be beneficial if there are specific points along the curve more likely to be stable
  - **Ride the yield curve**
    - This strategy involves selling bonds as they approach maturity, and then buying new bonds to repeatedly increase the duration of the portfolio
    - To optimise this strategy, investors should select bonds at the peak of the steepest portion of the curve, selling the bond once it has "rolled down" this portion
  - **Carry trades**
    - This is a more advanced strategy that utilises leverage to enhance returns
  - **Adjust portfolio convexity**
    - If yield curve shifts are large, convexity enhances returns and reduces losses
    - However, higher convexity assets usually have lower yield
    - Convexity is a second order effect, and so yield shifts must be significant for benefits to outweigh costs
  - **Adjust portfolio duration**
    - As duration increases, the inverse relationship between a change in yields and a change in prices strengthens
    - For a decrease in rates, reduced duration is optimal
    - For an increase in rates, increased duration is optimal
  - **Bullet vs. Barbell vs. Ladder**
    - In general, exposure should be increased where rates are expected to fall, and decreased where rates are expected to rise
    - This should be done within the constraints of desired total portfolio duration
    - A bullet portfolio concentrates exposure at one point in the curve, close to total desired duration
    - A barbell portfolio concentrates exposure at longer and shorter points on the curve
    - A laddered portfolio evenly distributes exposure along the curve

## 24.B: Explain how to execute a carry trade

- A carry trade at its simplest involves financing investment at a higher rate, by borrowing at a lower rate
  - If the yield curve is stable and slopes upward, borrowing at short-term rates and investing at long-term rates generates a return
    - If the curve isn't stable, and short term rates increase, the cost of borrowing can overtake the return
    - Additionally, if long term rates increase, the comparative value of the longer term bond purchases can fall
  - An alternative method is to invest in a higher interest rate currency
    - This trade involves similar risks to the previously described trade
    - Additionally, this trade exposes an investor to currency risk
      - If the invested currency falls in value, more will need to be purchased in order to settle the debt used to make the trade
    - A currency swap is an alternative approach, involving no initial net investment, only a risk neutral exchange of notional principals
    - The use of swaps provides an investor with additional flexibility in the way the trade is carried out
      - A long-term bond can be purchased in a higher yield currency, and used as collateral in a repo agreement to finance the purchase
      - The investor owns the bond and earns the return on it, whilst paying the shorter term interest rate in that same higher yield currency
      - As an alternative to paying in the same currency, the investor can enter into a currency swap to receive that higher yield currency, and pay a short term rate in a low yield currency in return

## 24.C: Explain why and how a fixed income portfolio manager might choose to alter portfolio convexity

- When significant changes in yields are expected, increasing convexity enhances returns and reduces losses
  - Modest changes in convexity can be achieved through the selection of a barbell
    - Other variables held constant, a barbell portfolio has higher convexity but lower yields, than a bullet portfolio
  - More dramatic changes in convexity can be achieved using options
    - Buying long calls and puts on bonds increases upside and reduces downside respectively, increasing convexity
    - Conversely, selling these options decreases convexity
    - A callable bond can be thought of as a combination of an option-free bond, and a short call on the bond, giving it negative convexity
    - Mortgage backed securities have characteristics similar to that of a callable bond
      - Since a fall in rates increases incentives to prepay, price upside is limited, reducing convexity
    - A putable bond can be thought of as a combination of an option-free bond, and a long put on the bond, giving it positive convexity

## 24.D: Formulate a portfolio position strategy given forward interest rates and an interest rate view

- Consider an investor attempting to design a portfolio, from a selection of five government bonds, for a one year holding period
  - In assessing the available options, the following calculations may be necessary:
    - **Rolldown price**, the projected price of the bond in one year, assuming no changes to the yield curve
      - This is a simple time of money problem, computing a present value given:
        - A future value (simply the par value)
        - An interest rate (this can be the yield of a bond one year closer to maturity, using the yield curve)
        - A coupon payment
        - A holding period (1 year in this case)
    - **Holding period return (or yield)**, simply computed as cash inflows divided by cash outflows
      - $\text{HPY} = \frac{\text{price}_f + \text{coupon}}{\text{price}_i} - 1$
      - Note that rolldown price can be used in place of $\text{price}_f$
    - **Manager forecast yield**, the managers predicted change in yields for each point on the yield curve
      - This is normally expressed in terms of a basis point shift for each key rate
    - **Manager's forecast of price**, the projected price given the manager forecast yield
      - The calculation is identical to that of rolldown price, but it takes account of the forecast yields, instead of assuming that the curve will remain unchanged
    - **Implied forward yield**, the forward yield that would generate the same one year holding period return as purchasing a bond immediately for the same time period
      - For example, a bond trading at its two year implied forward yield, would generate the same return as immediately purchasing a two year bond at its spot rate
      - These yields are calculated from spot rates, which are in turn calculated from par bond YTMs
        - Alternatively the spot rates can be calculated through *bootstrapping*
          - Given a one year bond that pays par value $P$, plus a coupon $C_1$, and a two year bond that pays $C_2$, the spot rate $S$ is given by:
$$
\frac{C_2}{C_1} + \frac{P + C_s}{(1 + S)^2} = P
$$
      - This approach can be repeated to continue determining spot rates for bonds of greater maturities
        - Once these rates have been calculated, the implied forward rates can also be calculated
        - To calculate a forward rate for a $j$-year bond in $k$ years $f_\text{j, k}$, the spot rates $S_\text{j}$ and $S_\text{k}$ are used:
$$
(1 + f_\text{j, k}) = \frac{(1 + S_\text{j})}{(1 + S_\text{k})}
$$
    - Finally, the **implied forward yield change**, the forward rate versus the spot rate
  - With this data in hand, there remain several approaches
    - One, is to assume the yield curve is likely to remain unchanges
      - This approach would entail using the holding period return given the rolldown price assuming no yield changes
    - A second approach involves trusting the manager yield forecast, and use a holding period return calculated from that forecast
      - An alteration to this approach involves comparing the forecast yields with the implied forward yields

## 24.E: Explain how derivates may be used to implement yield curve strategies

- Adjusting portfolio duration can be difficult, and costly, given the low liquidity in the bond market
  - Derivatives offer an alternative route, that can be more efficient
  - Additionally, they are particularly apt for temporary adjustments, since they tend to have shorter terms than bond instruments
    - In the case of parallel yield curve shifts, all strategies that change duration equally should be expected to perform equally
    - For non-parallel shifts, strategies that increase durations at maturities likely to see a fall in yields, and decrease durations at maturities likely to see a rise in yields perform best

- Bond futures contracts can be used to increase duration
  - Shorting them can decrease duration
  - The point on the yield curve at which duration is increased depends on the maturity of the bond the contract is for
  - In order to achieve a desired shift $\Delta \text{PVBP}$, the number of futures $N_f$ required can be calculated using the following:
$$
N_f = \frac{\Delta \text{PVBP}}{\text{PVBP}_f}
$$

- A receive-fixed, pay-floating swap increases duration
  - Conversely, a pay-fixed, receive-floating reduces duration
  - The notional principal required in order to achieve a desired shift in $\text{PVBP}$ can be done in a similar way as for futures
  - The point on the yield curve at which duration in increased depends on the length of the swap

## 24.F: Evaluate a portfolio's sensitivity to a change in curve slope using key rate durations of the portfolio and its benchmark

- A **key rate duration** (or **partial duration**) indicates the change in price given a shift in yields at one specific point on the yield curve
  - Key rate durations at multiple points on the curve can be combined to more precisely estimate the impact of shifts to a specific new curve
  - Given an expected curve, this can be expressed as a group of expected shifts at each point
  - Each expected shift can be multiplied by the key rate duration at that maturity, and then by the fixed income value at each maturity
  - This would give an estimated change in portfolio value given a shift to a specific new estimated curve

## 24.H: Construct a duration-neutral govenment bond portfolio to profit from a change in yield curve curvature

- Consider a choice between three portfolios of identical duration
  - A laddered portfolio
  - A bullet portfolio
  - A barbell portfolio
- If the curve is steepening, the bullet is optimal since it has the least exposure to the significant rate increases at the far end of the curve
- If the curve is flatterning, the barball is optimal since it has the most exposure to the significant rate decreases at the far end of the curve
- If the curvature is increasing (intermediate rates increasing, long and short term rates static), the barbell is optimal, with no exposure to rate increases
- If the curvature is decreasing, the bullet is optimal, with the most exposure to the rate decreases

- **Butterfly trades** make use of leverage to generate return from shifts in curvature
  - For example, shorting intermediate bonds, and investing in both short and long term bonds is effectively a *super barbell*
  - The long and offsetting short position offset each other for zero duration
  - No investor capital is required since the proceeds from the short finance the long
  - There is also net positive convexity due to cash flow dispersion
  - A **condor** trade is similar to a butterfly trade, with the difference being that two intermediate term bonds are used instead of a single bullet

## 24.G: Discuss inter-market curve strategies

- In addition to the strategies already discussed, managers can also invest across markets
  - An investor can have unique yield curve expectations for each market
  - Intra-market strategies include:
    - A swap with payments made in the domestic currency, that entails receiving a rate at the steeper end of a yield curve, and paying a rate at the flatter portion of a curve
    - Alternatively a bond can be bought at one end of the curve in one market, and shorted at the other end of the curve in another market

## 24.I: Evaluate the expected return and risks of a yield curve strategy

- In general, understanding the effect of a change to the yield curve involves analysing each source of return over a given period
  - Coupon payments
  - Rolldown return
  - Returns from changes in the curve
  - Currency fluctuations