---
sequence: 25
title: 'Reading 25: Fixed Income Active Management Credit Strategies'
section: 9
sectionTitle: 'Fixed Income Portfolio Management'
layout: reading
---

# Reading 25: Fixed Income Active Management Credit Strategies

## 25.A: Describe risk cnsiderations in investment-grade and high yield corporate bond portfolios

- The **credit market** is the market containing all assets with non-zero credit risk
  - They can be public
    - Sovereign debt
    - Corporate debt
    - Supranational debt
    - Money market instruments
  - They can be private
    - Loans
  - Other assets such as MBSs can be public or private

- **Investment grade** assets are generally held to be those rated above *BB*
  - This is equivalent to Baa3+ for Moody's, and BBB- for Standard & Poor and Fitch Ratings
  - The remaining assets are referred to as *speculative*, or *junk* bonds

- Individual analysts may investigate deeper than public ratings, and consider the five Cs of credit analysis
  - Capacity to pay
  - Collateral
  - Covenants
  - Character of the issuer
  - Capital of the issuer

- A single bond can provide multiple types of risk exposure:
  - **Credit risk**, formed from **default risk** and **loss severity**
  - **Spread risk** is the risk of a fall in price relative to risk free bonds due to a widening of the spread
    - Modified duration is used in calculating a price change due to a general shift in interest rates
    - **Spread duration** is used in calculation a price change due to a change in spread
      - Most bonds have identical spread and modified duration
      - Floating rate bonds can have low modified duration but high spread duration
  - **Credit migration risk** is a fall in price due to an asset being recategorised
  - **Liquidity risk** is the risk of having to accept a below-market value due to the need to sell an asset quickly
    - wider bid-ask spreads and regulatory issues mean liquidity risk is most pronounced for high-yield securities

- Risk-free rates and spread often move in opposite directions
  - In strong economic conditions, risk-free rates rise, but spreads tighten as probability of default falls
  - In weaker conditions, the opposite is true
  - This means investors using investment grade securities are mostly exposed to interest rate risk
  - Investors using high-yield assets are mostly exposed to credit risk and spread risk

## 25.B: Compare the use of credit spread measures in portfolios

- There are several ways to measure credit spread
  - **Benchmark spread** is the difference between a bond's YTM, and that of a risk-free benchmark of a similar duration
    - The on the run government issue is normally used for this purpose
    - Due to a limited number of govenment bonds available for this purpose, linear interpolation between the two closest matches is used
    - This spread is the **G-spread**, and can be used to calculate a hedge of the interest rate risk whilst retaining the credit spread of a bond
      - By matching a long position in a corporate bond with a short position in government bonds, a return equal to the G-spread can be earned
    - The **I-spread** is calculated in a similar fashion but using swap fixed rates instead
      - This yields a smoother curve due to a greater abundance of rates available, however
        - They do not reflect fully risk free rates, especially not during times of economic hardship
  - The **Z-spread** is a trial and error calculation
    - It is the spread that, if added to implied initial spot rates of risk-free bonds, will discount the cash flows to the current market value
    - The **option-adusted spread (OAS)** is a version of the Z-spread that accounts for the impact of embedded options
      - Using an assumed interest rate volatility, an interest rate tree can be constructed, determining future cash flows
      - The OAS is then determined by trial and error such that if added to each node of the tree, cash flows are discounted to current market value
      - It is important to note that the OAS is an average rate that incorporates the multiple paths that a bond with an embedded option may take
      - Over time, rates will follow a single path, and the actual rate can shift significantly
      - If a portfolio includes a mix of bonds with and without embedded options, the OAS will be the best measure

- Credit spread can be interpreted as the return above the used benchmark
  - If the spread is stable then excess return is the spread
  - If the spread is not stable then the change in spread, as well as the spread duration will become important factors
    - If the spread widens, performance falls, and vice versa
    - Losses due to probability of default and loss severity can also be included in return measures
  - Therefore, excess return $\text{XR}$ can be estimated as a function of spread $\text{s}$, change of spread $\Delta \text{s}$, spread duration $\text{SD}$, time period $\text{T}$, a probability of default $\text{p}$, and a loss severity $\text{L}$:
$$
\text{XR} = (\text{s} \cdot \text{t}) - (\Delta \text{s} \cdot \text{SD}) - (\text{t} \cdot \text{p} \cdot \text{L})
$$

## 25.C: Discuss bottom-up approaches to credit strategies

## 25.D: Discuss top-down approaches to credit strategies

- Bottom-up strategies involve focusing specifically on the least efficient sectors to determine which securities may be incorrectly priced
  - They work best when comparing bonds with similar credit risk
  - However, changes in the portfolio can be dominated by macro factors such as interest rates
  
- Top down strategies focus primarily on the macro factors that drive things such as interest rates
  - However, these factors are closely observed by many, and it is difficult to achieve an informational advantage

- A combined approach can be acheived in two main ways
  - Build a portfolio that over or underweights individual securities according to bottom-up analysis
  - Then adjust the portfolio according to macro factors

- Bottom-up analysis involves a number of processes:
  - Divide the set of bonds available for investment into individual sectors
  - Determine the sector weights in the benchmark, and evaluate them for reasonableness
  - Identify inefficiencies and misvaluations within each sector to identify securities with potential
  - Assess credit risks by collecting default rates and loss rates
  - Plot spread curves for individual issuers
    - Higher spread, assuming other factors are equal, means a more attractive investment
    - Individual bonds issues that are above the curve are more attractive
  - In determining final allocations, evaluate spread duration and portfolio value allocation in tandem
    - For IG bonds, default is not considered likely, and hence spread duration is the most useful measure of risk
    - For HY bonds, actual value allocated is more important, due to increased likelihood of default
  - Due to the nature of fixed income, the desired issue may not be available
    - The investor can identify the next most suitable candidate
    - The investor can use an index fund, swaps, or derivates to replicate the desired exposure until the bond is available
    - The investor can simply hold cash and wait until the desired bond is available

- A top-down approach focuses on macro factors like economic growth, or corporate profits
  - This can also help identify sectors which are likely to face changing prospects and therefore have their weight adjusted
  - Historical patterns such as the credit cycle may also be used
  - Anticipating changes in economic conditions is vital in timing movements up and down in credit quality
  - The means of calculating average credit risk is important
    - Some methods assign numeric values to each risk rating that increase linearly
    - More complex methods use non-linear systems that assign progressively higher weights to riskier ratings

- Simultaneously managing credit risk and interest rate risk without derivatives can be difficult
  - If expectations are that spreads are likely to narrow, and rates are likely to increase, it would be difficult to invest appropriately with bonds alone
  - Adjusting option exposure through putable or callable bonds may be more difficult than using options on bond contracts

## 25.E: Discuss liquidity risk in credit markets and how liquidity risk can be managed in a credit portfolio

- The market for risky fixed income instruments is relatively illiquid compared to that of risk free instruments
  - Liquidity is also reduced following the crisis of 2008 and 2009
  - Credit spread is sensitive to trading volume flows
    - e.g. Flows to IG instruments from HY instruments would increase HY yields and reduce IG yields, widening spreads
  - Bid-ask spreads are often used as a measure of liquidity but more recently this has become less reliable
  - However, dispersion and distribution of the market has increased, with the ten largest funds holding a smaller percentage

- To manage liquidity risk, managers can
  - Hold more cash and cash equivalents
  - Make use of ETFs until desired securities become available
  - Make use of liquid derivatives to achieve similar exposure

## 25.F: Describe how to assess and manage tail risk in credit portfolios

- **Tail risk** reflects the way in which markets can experience more drastic declines than their standard deviation implies
  - Anticipating or modelling these declines is difficult
  - **Scenario analysis** can begin with an assumption of conditions that may be unusual
  - **Historical analysis** can use values from a previous crisis as inputs into a model

- During a crisis the benefits of diversification can fall dramatically as correlations increase
  - Liquidity dries up rapidly, and so managers can try to retain securities that maintain liquidity, even in these scenarios
  - If tail risks can be identified, also identify securities which may benefit if they come to pass

## 25.G: Discuss considerations in constructing and managing portfolios across international credit markets

- Restricting a credit portfolio to domestic bonds does not isolate an investor from global opportunities and risks
  - The issuers often have international operations

- The emerging market (EM) sector has increased in size to almost match the US HY sector
  - Commodities and banking make up a significant proportion of the EM sector
  - State ownership of issuers is common
    - Whilst this creates an implicit expectation that they will step in to ensure creditworthiness, there is also the risk that domestic creditors will take priority
  - The rating giving to a corporate EM bond may be understated since some ratings agencies will not allow it to exceed the rating given to the government of that state

- Liquidity is a greater issue in the EM market
  - The US sector has transparency and public reporting on trade volumes and prices, encouraging further trade

- Trading internationally introduces currency risk
  - This is particularly pronounced for low yield bonds, since in those cases currency return is a larger proportion of total return

- With less developed or familiar legal and regulatory structures, there can be significant legal risk

## 25.H: Describe the use of structured financial instruments as an alternative to corporate bonds in credit portfolios

- Structured finance instruments can function as an alternative to corporate bonds
  - They have higher yields
  - Tailored risk exposures
  - Specific sector exposures
  - Diversification benefit

- A **mortgage backed security (MBS)** is a pool of mortgage-backed loans
  - They offer similar yields to corporate bonds
  - Higher liquidity than corporate bonds
  - Tailored exposures to portions of the real estate market (e.g. commercial or residential)
  - Provide exposure to interest rate volatility due to the prepayment option in most mortgages
    - Prepayment is more likely if interest rate volatility increases
    - If an investor expects lower volatility, they can increase exposure to that volatility by purchasing more MBSs

- **Asset backed securities (ABS)** are similar, collateralised with other debt such as car loans, credit card receivables, or student loans

- **Collateralised debt obligations (CDO)** are usually backed by a form of corporate debt, arranged into tranches
  - Senior tranches are paid first
  - Credit quality falls, the less senior the tranche
  - Provide opportunities for investors to identify misvaluation compared to the underlying collateral
  - Leveraged exposure
    - An investment in the lowest tranches is equivalent to a leveraged investment in the corporate debt underlying it