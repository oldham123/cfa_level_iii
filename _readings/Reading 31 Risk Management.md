---
sequence: 31
title: 'Reading 31: Risk Management'
section: 12
sectionTitle: 'Risk Management'
firstReading: true
layout: reading
---

# Reading 31: Risk Management

## Secret Sauce Notes

- Risk management is a process that is always *ongoing*, and involves:
  - Identifying and quantifying exposures
  - Setting tolerances
  - Reporting exposures to stakeholders when necessary
  - Monitoring portfolios and taking corrective actions
  - Addressing it as frequently as possible is ideal

- **Risk governance** is the component of governance involving developing and implementing a risk management system
  - *Decentralised* risk governance calls upon individuals to manage risk
  - *Centralised* risk governance takes more of a firm-wide approach to risk

- Specific risks include, but are not limited to:
  - Market risk
  - Liquidity risk
  - Settlement risk
  - Credit risk
  - Operations risk
  - Model risk
  - Sovereign risk
  - Regulatory risk
  - Political risk
  - Tax risk
  - Accounting risk
  - Legal risk

- In evaluating a risk management system, it is important to consider:
  - Is capital allocated in respect of risk?
  - Are relevant risks identified by the system?
  - Is the model for quantifying risk appropriate?
    - Are correlations of risk factors considered?
    - Does the model allow for changing factor sensitivities
  - Are risks managed effectively?
    - Is there a distinction between risks that can be managed, and risks that must be hedged?
  - Is there a committee with the duty of monitoring the system as a whole?
  - Are there built-in controls?
    - Does it feature continual monitoring of risk factors?
    - Can new risks be included?
    - Does the system monitor itself?

- **Market risk** refers to the changing of values such as interest and exchange rates, as well as asset prices
  - **Standard deviation** is a common measure of risk
  - When standard deviation is measured relative to that of a benchmark, it is called *active risk*, *tracking risk*, *tracking error volatility*, or *tracking error*
  - Excess return over a benchmark is *active return*
    - The ratio of active return over active risk is the **information ratio**

- Non-financial risk is so hard to quantify that often it will not be attempted
  - The more common approach is simply to buy insurance

- **Value at risk (VaR)** is an estimate of the minimum expected loss:
  - Over a given time horizon
  - At a given significance level
  - VaR for a portfolio cannot be calculated without considering asset correlations
  - It is important to note that the accuracy of VaR as a risk measure can only be determined after the fact
  - Methods for calculating it include:
    - Use of historical data
      - When calculating at a given significance percentage, take that percentage of the lowest returns, and then select the highest return of that subset
      - Multiply by portfolio value to get historical VaR
      - The historical method requires a large amount of data
      - It also assumes that the past will be a reliable guide to the future
    - Use of Monte Carlo simulation
      - Requires less data than the historical method
      - Also assumed the past is a good indicator
    - Use of the **analytical method**
      - For a portfolio with an expected daily return of $\hat{\text{R}}_p$, a daily standard deviation of $\sigma$, a value of $\text{V}_p$, and a critical value given by the chosen significance level of $\text{z}$, VaR is given by:
$$
\text{Daily VaR} = \left( \hat{\text{R}}_p - \text{z} \cdot \sigma \right) \cdot \text{V}_p
$$
where
$$
\sigma_\text{daily} \approx \frac{\sigma_\text{annual}}{\sqrt{250}};\text{ }\sigma_\text{monthly} \approx \frac{\sigma_\text{annual}}{\sqrt{12}};\text{ }\sigma_\text{daily} \approx \frac{\sigma_\text{monthly}}{\sqrt{22}};
$$

- VaR is useful in that it is relevant regardless of the type of assets
  - However, it fails to capture the potentiality of extreme losses

- In order to calculate analytical VaR for a portfolio of two assets, first:
  - Calculate the weighted average of expected returns of each asset
  - Calculate the combined variance of the portfolio using the two-asset portfolio variance formula

- **Incremental VaR** expresses the impact on VaR of a specific change to a portfolio (i.e. adding a new security)
  - **Cash flow at risk** is the same technique applied to cash flows, similar to **earnings at risk**
  - **Tail value at risk** tries to account for potential losses in the tail end of the distribution
  - It is important to note that VaR does not account for liquidity, which could exacerbate losses

- VaR should be combined with **stress testing** and **scenario analysis**
  - These techniques help to understand the potential impact of more extreme scenarios
  - **Factor push analysis** pushes either a factor, or a group of factors into extreme regions to measure the likely effect
  - **Maximum loss optimsation** is the process of identifying factors with the greatest potential to impact portfolio value

- Exposure to **credit risk** is a function of the *probability of default*, and the *severity of the loss* (if it occurs)
  - **Current credit risk** refers to payments already due
  - **Potential credit risk** refers to payments due in the future
  - **Credit VaR** is the expected loss due to default with a given probability during a time perod
    - It applies to assets which entitle the owner to future cashflows from a counterparty who may potentially default
  - The value (and therefore credit risk) of a forward contract is given by:
$$
\text{V}_\text{forward} = \frac{\text{spot}}{(1 + \text{foreign})^t} - \frac{\text{forward}}{(1 + \text{domestic})^t}
$$
  - The credit risk of a swap is simply the difference between the received and paid present values
  - Option credit risk is borne by the long

- **Risk budgeting** is the determination of total acceptable risk, and then the allocation of that risk across components of a firm
  - An ERM system allows the risk budget to be monitored continuously, whilst also monitoring performance
  - A **position limit** simply caps the positions that managers can take
  - **Liquidity limits** are position limits related to trading frequency
  - A **performance stopout** is a dollar limit for losses over a given period

- Credit risk can be managed in several ways
  - Limit exposure to a single debtor
  - Mark to market
    - This is used when one party has obligations to another, and involves settling credit risk based on the current status of those obligations
  - Netting
    - This is used when two parties have obligations to each other, and involves netting those obligations off one another so that credit risk on one party is reduced, and the other becomes zero
  - Use of collateral
  - Use of special purpose vehicles and enhanced derivatives products companies
    - An SPV allows parent companies to engage in transactions that they otherwise could not
    - They are capitalised in such a way as to secure a high credit rating
  - Transfer risk to other investors

- Risk adjusted performance can be measured in the following ways:
  - Sharpe ratio
  - Information ratio
  - Risk-adjusted return on invested capital
  - Return over maximum drawdown $\rightarrow \frac{\bar{R_p}}{\text{maximum drawdown}}$
  - Sortino ratio $\rightarrow \frac{\bar{R_p} - \text{MAR}}{\text{downside deviation}}$
    - The motivation behind the Sortino ratio, is that strong performance can inflate measures of volatility
    - This means that if standard deviations are used as a performance indicator, high performing managers can be punished

- **Nominal position limits** are alocations of dollar amounts
  - Their use has several drawbacks:
    - The impact of correlations between each position is not captured
    - It is possible to exceed limits by combining assets (especially derivatives)
    - **VaR position limits** improve on this, but still don't capture correlations
    - A **maximum loss limit** can be used to set a theoretical maximum loss the firm needs to be able to endure