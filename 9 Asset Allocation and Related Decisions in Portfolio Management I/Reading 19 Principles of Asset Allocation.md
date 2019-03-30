# Reading 19: Principles of Asset Allocation

## 19.A: Describe and critique the use of mean-variance optimisation in asset allocation

- **Asset allocation** is the process of establishing the weights of each asset class within the portfolio
  - **Implementation decisions** are the specific choices of asset to include within the portfolio

- **Mean-variance optimisation** is an asset-allocation apprach that aims to provide maximum return for a given level of risk
  - Its inputs include:
    - A set of assets which may be included in a portfolio
    - Risk and return expectations for each asset
    - Correlations between each pair of assets
  - The set of allocations produced form the **mean-variance efficient frontier**, each giving the greatest return for each risk level
  - Once the frontier has been established, the appropriate portfolio must be selected from it
    - One approach to this is to make use of a utility function, with the aim of maxmimsing utility:
$$
U_m = \text{E}(R_m) - \frac{\lambda \cdot \sigma^2_m}{2}
$$
  - This function captures the nature of an investor's utility to increase with return, and decrease with risk
  - $\lambda$ denotes the investor's individual preference for accepting additional units of risk in order to generate additional units of return
    - A truly **risk neutral** investor would have a value of 0, but it is more common to use a value between 1 and 10, with an average of 4

- MVO is, at its core, an optimisation problem, where a certain value is maximised subject to contraints, including:
  - Asset-allocation weights
  - The *budget constraint* requiring that weights sum to 100%
  - The *non-negativity constraint* requiring that weights are between 0% and 100%
  - Other investor specific constraints
    - Note that if too many additional constraints are applied, then the value of optimisation is reduced

- Disadvantages of MVO include:
  - Dependence on the quality of inputs
  - Veers towards portfolios highly skewed towards some asset classes, with little to no allocation to others
  - Neglects skew and kurtosis in asset returns, despite empirical demonstration that both are present
    - It is possible to extend MVO in order to account for additional inputs by adjusting the utility function, or by using a different risk measure
  - Different asset classes may still give exposure to the same risk factors
  - Neglects the liabilities that a portfolio may be intended to eventually fund, and the correlations between those liabilities and returns
  - Takes a single period view, and therefore neglects the costs of rebalancing

- Since poor return estimates are a large source of error in MVO, improving those inputs is usually a worthwhile exercise
  - **Reverse optimisation** is a possible way of doing that
    - Begin with optimal weights from the global portfolio
    - Determine asset returns consistent with those weights
    - Input these implied returns into MVO to generate optimal weights for an individual investor
  - This process assumes that the global portfolio is diversified
    - Since these returns are derived from a diversified portfolio, this can also address the problem of MVO recommending highly concentrated positions
  - **Black-Litterman** is an adjustment to reverse optimisation which includes further adjustment of implied returns in order to account for specific return expectations that an investor may have

- **Resampling** involves applying Monte-Carlo techniques to MVO
  - Generate an efficient frontier using initial best estimates of the inputs
  - Generate distributions of randomised inputs around those best estimates, generating a set of efficient frontiers
  - Combine these to create a *resampled efficient frontier* which averages the individual frontiers

## 19.C: Interpret and critique an asset allocation in relation to an investor's economic balance sheet

- The MVO approach can be adapted in order to account for non-financial assets, such as human capital, or real estate
  - Income from employment can be modelled as an inflation-linked bond
    - If income is more volatile, such that this is inappropriate, equities or corporate bonds can be added into the model
  - This allows capabilty to take on risk to be raised, in accordance with an investors true characteristics
    - It is important to recall that since human capital is not a tradeable asset, it's proportion within the final allocation is fixed
  - Real estate can be encorporated in a similar way using reference to a real estate index

## 19.G: Discuss the use of Monte Carlo simulation and scenario analysis to evaluate the robustness of an asset allocation

- Monte Carlo simulation has multiple applications in asset allocation decisions
  - Account for complications of multi-period investing, including rebalancing, and tax consequences
  - Illustrate the consequences of different risk tolerances to guide investors to selecting the best risk levels for them

## 19.D: Discuss asset class liquidity considerations in asset allocation

- It is difficult to include illiquid asset classes into MVO
  - There is a lack of availablity of good data required to make reliable estimates regarding return, risk, and correlation
  - Passive investment in the indices that exist are usually not comparable to active investment
  - Specific investments into illiquid assets generally do not share the risk and return profile of the class as a whole

- To address these concerns:
  - Exclude such illiquid asset classes from the MVO process
  - Include illiquid asset classes but specifically model the characteristics of the actual investments planned
  - Include inputs from a highly diversified alternative investments index, whilst being mindful that the actual investments made may differ

## 19.E: Explain absolute and relative risk budgets and their use in determining and implementing an asset allocation

- The goal of risk budgeting is to ensure that the maximum amount of return is generated per unit of risk taken
  - **Marginal contribution to portfolio risk (MCTR)** is the change in risk given a small change in the allocation of an asset class
    - $\text{MCTR}_i = \beta_i \cdot \sigma_M$
  - **Absolute contribution to total risk (ACTR)** is the total risk contribution from the allocation to an asset class
    - $\text{ACTR}_i = \text{weight}_i \cdot \text{MCTR}_i$
  - Using the MCTR of each asset class, the impact on portfolio risk as the allocation to each class changes is easily observed
  - This allows for the indentification of optimal allocations
    - Optimal allocations are those where $\frac{R_i - R_F}{\text{MCTR}_i}$ is equal for all $i$

## 19.F: Describe how client needs and preferences regarding investment risks can be incorporated into asset allocation

- The risk preferences of investors can be incorporated in the following ways:
  - Allowing the investor to specify additional constraints
  - Determine a risk averision factor to be used in a utility function when applying MVO
  - Apply MCS to illustrate to an investor the implications of multiple risk choices

## 19.H: Describe the use of investment factors in constructing and analysing an asset allocation

- The MVO process can also be used to identify optimal exposures to multiple risk factors, in place of asset classes
  - These include:
    - Exposure to a market
    - Firm size
    - Firm value
    - Price momentum
    - Liquidity
    - Interest rate risk
    - Creditworthiness
    - Variance
  - The choice of whether to apply MVO using asset classes or risk factor exposures depends mostly on that which an investor is most familiar, and most comfortable forming capital market expectations

## 19.J: Describe and evaluate characteristics of liabilities that are relevant to asset allocation

- When considering asset allocation, and attempting to account for investor liabilities, it is important to consider the following:
  - Do the liabilities have fixed cash flows, or are they contingent on future events?
  - Do the liabilities represent legal obligations on the part of the investor?
  - What are the duration and onvexity characteristics of the liability?
  - How large is the liability relative to the total assets owned by the investor?
  - What may influence the future cash flows?
  - Are the liabilities subject to regulations?

## 19.K: Discuss approaches to liabilitiy-relative asset allocation

## 19.L: Recommend and justify a liability-relative asset allocation

- **Surplus optimisation** is an alteration to MVO in which an efficient frontier is defined by the surplus, using the variance of that surplus as the risk measure
  - Surplus return $R_s = \frac{\left(\Delta \text{portfolio value} - \Delta \text{liability value}\right)}{\text{initial portfolio value}}$
  - This can then be substituted into the utilty function
  - Determining risk and return profiles for liabilities can be done by either modelling them as corporate bonds, or by using a risk factor approach

- The **two-portfolio** approach involves dividing the total portfolio into two subportfolios
  - One is designed to hedge the investor's liability
  - The other is managed with an MVO approach to generate additional return
  - Modifications to the approach are possible:
    - Allocate more capital to the return-seeking subportfolio
    - Allocate more capital to the hedging subportfolio
  - Limitations include:
    - Hedging portfolios are difficult to construct effectively before the liability is fully funded
    - Some unique risks faced by insurance firms are either difficult, or impossible to hedge against (e.g. natural disasters)

- The **integrated asset-liability approach**
  - If the liabilities held by the investor are not fixed, and involve decisions to be made in response to portfolio performance, then they can be integrated into the portfolio itself as an asset class
  - An example of an investor that may need to take this approach is a bank

## 19.M: Recommend and justify an asset allocation using a goals-based approach

- For investors with multiple aims, each with different priorities and time horizons, a goals-based approach may be appropriate
  - Portfolios are divided into subportfolios, with each targeting a specific goal
  - Each subportfolio aims to provide a minimum expected return necessary to confer a specified probability of success of a goal
  - Advisors may have subportfolios ready to meet various goals, rather than customising them for every client
    - These may be referred to as *modules* with each having certain risk-return profiles, liquidity characteristics, and asset classes
  - Given a desired probability of success, the module with the highest expected return is selected
    - The amount invested into that module is the amount demanded by the goal, discounted at the expected rate of return

## 19.N: Describe and critique heuristic and other approaches to asset allocation

- "**120 minus your age**" is an approach designed to estimate an appropriate allocation to equities based on the age of the investor
  - Whilst this approach is not sophisticated, it successfully reflects the fact that human capital declines as investors age, requiring their financial capital to be reallocated from equity-like investments to bond-like investments over time
  - Additionally, it often comes close to the recommendations of more sophisticated approaches

- **60/40 split** simply advocates maintaining 60% to 40% allocation between equities and bonds
  - This is reasonably close to the allocations within the global market portfolio

- The **Endowment / Yale model** advocates larger investments in alternative asset markets
  - These markets are less efficient and so there are opportunities for excess return
  - In addition, investors with longer time horizons can tolerate the high liquidity risk of these investments in return for a liquidity premium

- The **Risk Parity** approach advocates insuring that each asset class constributes the same amount of risk to the overall port
  - Whilst this approach avoids an MVO approach from recommending highly concentrated positions, it also ignores return characteristics

- The **$\frac{1}{N}$ rule** advocates simply allocating equally to all classes
  - Empirical evidence suggests that this approach performs surprisingly well, but not optimally

## 19.O: Discuss factors affecting reblancing policy

- Rebalancing of portfolios may be needed for several reasons:
  - Changing investor goals
  - Changing market conditions or expectations
  - Realigning a portfolio to agreed upon asset allocations

- Percentage-range rebalancing is an approach that determines *corridors* around the intended allocation for an asset class, and if market movements send the allocation outside that corridor then that triggers rebalancing
  - Determining the optimal size of that corridor involves considering a number of factors:
    - Transactional costs incurred by rebalancing
    - Tolerance of the additional risk created as some allocations naturally fluctuate
    - Correlation of the asset class with the portfolio as a whole
    - Asset class volatility