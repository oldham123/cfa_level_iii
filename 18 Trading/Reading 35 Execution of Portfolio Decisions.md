# Reading 35: Execution of Portfolio Decisions

## Secret Sauce Notes

- A **market order** is an instruction to execute a trade immediately at the best price currently available
  - If the entire order cannot be completed at a single price, it will be filled in by consecutively less attractive prices
  - This method offers *speed* and *uncertainty*

- A **limit order** will only trade at a prespecified price or better
  - If not fulfilled, the trade expires
  - This method has *execution uncertainty*

- **Effective spread** compares the actual achieved price against the **midquote**, and then doubles the difference
  - The midquote is the price at the center of the **inside bid-ask spread**
  - The inside bid-ask spread is the spread implied by the best bid (**inside bid**) and the best ask (**inside ask**) on the market

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
  - Implicit costs include losses due to spreads, marke impact costs, opportunity costs, and slippage
  - **Volume weighted average price** is the executed trade price of a security compared to the weighted average of trade prices for a security during a day of trading
  - **Implementation shortfall (IS)** measures transaction costs by comparing actual performance to that of a hypothetical portfolio that executes all trades costlessly
    - It can be expressed as a total dollar amount, an amount per share, or a basis point amount by dividing by the value of the order
    - It is important to note that some tades are not executed in a timely manner, and others never execute at all
    - These events would necessitate adjustments to an IS calculation
      - *Decision price* is the price at which an order initiates
      - *Execution price* is the price at which an order executes
      - *Revised benchmark price* is the price of the security if the trade isn't completed sufficiently quickly
      - *Cancellation price* is the price of the security if the trade is cancelled
    - Total IS is the difference between portfolio value after the trade, and hypothetical value after the trade is completed fully at the decision price, divided by the hypothetical portfolio investment
    - **Missed trade** is the difference between cancellation and decision prices, multiplied by order volume
    - **Delay (slippage)** is the difference between revised benchmark price and decision price, multiplied by trade volume
    - **Market impact** is the difference between execution and decision prices multiplied by trade volume