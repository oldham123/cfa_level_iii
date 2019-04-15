#Reading 24: Yield Curve Strategies

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

- Optimal strategy is not always clear and may require futher analysis
  - A simple approach may be to simply assume that the yield curve will remain unchanged
  - A more complicated approach involves relying on some expectation of movement in the yield curve
  - More complicated still, expectations of yield curve movements can be combined with implied forward yields