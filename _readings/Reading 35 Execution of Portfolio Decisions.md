---
sequence: 35
title: 'Reading 35: Execution of Portfolio Decisions'
section: 14
sectionTitle: 'Trading'
firstReading: true
layout: reading
---

# Reading 35: Execution of Portfolio Decisions

## Secret Sauce Notes

- A **market order** is an instruction to execute a trade immediately at the best price currently available
  - If the entire order cannot be completed at a single price, it will be filled in by consecutively less attractive prices
  - This method offers *speed* and *uncertainty*

- A **limit order** will only trade at a prespecified price or better
  - If not fulfilled, the trade expires
  - This method has *execution uncertainty*

- The *size* of the bid or ask is referring to the number of shares being offered or sought by the market

- **Effective spread** compares the actual achieved price against the **mid-quote**, and then doubles the difference
  - The mid-quote is the price at the center of the **inside bid-ask spread**, or the **quoted spread**
  - The inside bid-ask spread is the spread implied by the best bid (**inside bid**) and the best ask (**inside ask**) on the market
  - If the effective spread is tighter than the quoted spread, this is a sign of *price improvement*

- Security markets offer three main advantages to investors:
  - **Liquidity**
    - A liquid market has three main advantages for investors:
      - Tight spreads, meaning investors can trade with fewer transaction costs
      - **Market depth**, allowing even large orders to take place without dramatically shifting the market
      - **Resilience**, causing prices to move quickly to eliminate deviations from intrinsic values
  - **Transparency**
    - This allows investors to inform themselves about the nature of the market both before and after trading
    - This increases confidence, and encourages participation
  - **Assurity of completion**
    - This allows investors to be confident that the counterparty to their trades will honour their obligations
  - Security markets come in three main forms:
    - **Quote driven markets**: Investors and dealers trade
    - **Order driven markets**: Investors trade without intermediaries
    - **Brokered markets**: Investors use brokers to find counterparties
    - Hybrid markets combine aspects of the previous three

- Costs of trade execution can be both *implicit* and *explicit*
  - Explicit costs include commissions, taxes, and fees
  - Implicit costs include losses due to spreads, market impact costs, opportunity costs, and slippage
  - **Volume weighted average price** is the weighted average of security prices during a day
    - VWAP is easy to understand and compute
    - However, it fails to account for delayed, or unfilled orders, or market movements or trade volume
    - By comparing the VWAP against an actual execution price, the implicit costs of that trade can be estimated
  - **Implementation shortfall (IS)** measures transaction costs by comparing actual performance to that of a hypothetical portfolio that executes all trades costlessly
    - IS as a measure of trading costs is preferable both to VWAP and effective spread, which can both be gamed by traders
    - It can be expressed as a total dollar amount, an amount per share, or a basis point amount by dividing by the value of the order
    - It is important to note that some trades are not executed in a timely manner, and others never execute at all
    - These events would necessitate adjustments to an IS calculation
      - *Decision price* is the price at which an order initiates
        - If an order is placed during market close, the decision price is the close of the previous day
      - *Execution price* is the price at which an order executes
      - *Revised benchmark price* is the price of the security if the trade isn't completed sufficiently quickly
      - *Cancellation price* is the price of the security if the trade is cancelled
    - Total IS is the difference between portfolio value after the trade, and hypothetical value after the trade is completed fully at the decision price, divided by the hypothetical portfolio investment, and can be expressed as the sum of:
      - Explicit costs, given by commission, divided by the hypothetical costless investment
      - Realised profit and los is given by the difference between the execution price, and either the decision price or revised benchmark price, divided by the decision price and weighted by the proportion of the order filled
      - **Missed trade**, the difference between cancellation and decision prices, multiplied by the portion of the order not filled
      - **Delay (slippage)**, the difference between revised benchmark price and decision price, multiplied by proportion of the order filled
      - **Market impact**, the difference between execution and decision prices multiplied by trade volume
    - IS can express the tradeoff between rapid execution and market impact
    - IS decomposes various contributions to trade cost more accurately
    - IS can be difficult to compute and interpret
  - The final price of execution can be affected both by implicit and explicit trading costs, as well as market movement
    - In order to gain an accurate picture of execution quality, these market movements should be stripped out of the IS measure
    - Using market return and beta (neglecting alpha over small time periods), this can be subtracted from an initial implementation shortfall cost to get an adjusted value

- Traders can be thought of as being information, or liquidity motivated
  - Both types will prioritise controlling the time at which their trades execute, and use market orders
  - Alternatively, value-motivated, or passive traders prioritise controlling the price at which their trades execute, and use limit orders

- The following are examples of trading tactics:
  - *Liquidity-at-any-cost*
    - Fast execution, but high costs and market impact, potentially leaking information
    - This method is likely to be favoured by information traders, who need to execute trades quickly before opportunities close
  - *Costs-are-not-important*
    - Fast execution at market price, but incurring larger trade costs
  - *Need-trustworthy-agent*
    - Skillful, slow execution to achieve a higher price, incurring higher commission costs and potentially leaking information
  - *Advertise-to-draw-liquidity*
    - Achieves the market price, but incurs higher administrative costs and possibly causes front-running
  - *Low-cost-whatever-the-liquidity*
    - Prioritises minimal trading costs, but leads to uncertain, and possibly unfavourable timing of the trade
      - Momentum markets can be problematic for these traders, because the moment of prices in a prevailing direction means that the price on a limit order may never be reached, with orders going unfilled

- **Algorithmic trading** is automated trading with the objective of minimising trade costs, and comes in three main forms:
  - *Logical participation*
    - **Simple logical participation strategies** seek to trade in a way that disguise the intentions of the investor amongst regular trade flow, using the value-weighted or time-weighted average price
      - This approach is suitable for trades with low urgency
    - **Implementation shortfall strategies** focus on trading quickly to minimise IS
      - Urgent trades are best suited to this strategy
  - *Opportunistic*
  - *Specialised strategies*

- The development of complex trading techniques and the decline of explicit trading costs has increased both the opportunity and incentive to act unethically
  - Buy-side traders should prioritise their clients over their relationships with sell-side traders
  - The increased anonymity of modern trading has created the opportunity to gain information from one trader and use it discreetly against them

- **Quote driven** markets offer liquidity
  - Traders interact with dealers posting bid and ask prices (also called **dealer markets**)
  - Dealers maintain inventories, and provide liquidity
  - Markets for illiquid securities are often dealer markets so that liquidity is improved
  - Dealers also provide liquidity for negotiated securities, such as swaps or forwards
  - The dealer offering the best price might still have undesirable credit risk, and so trades go elsewhere
  - Some dealer markets are **closed-book**, requiring the services of a broker

- **Order driven** markets offer best prices
  - Traders transact with other traders without intermediaries
  - Prices are set by supply and demand, but liquidity is likely to be less than in a quote driven market
  - Execution is determined by some mechanical rule, matching prices between buyers and sellers
  - Order driven market types include:
    - **Electronic crossing networks**
      - The typical trader is an institution
      - Orders are batched and "crossed" at fixed points in time over the day at average prices
      - Costs are low, but trades may go unfilled
      - The identity of the counterparty is usually unknown, and hence there is no price discovery, also causing trades to go unfilled
    - **Auction markets**
      - Traders submit orders that compete against others for execution
      - Trades can be periodic and batched, or continuous
      - These markets feature price discovery
    - **Automated auctions** (or **electronic limit-order markets**)
      - These markets trade throughout the day
      - Trades are executed according to a set of rules
      - They are computerised, and counterparties usually remain unknown
      - They are however auction markets, and provide price discovery