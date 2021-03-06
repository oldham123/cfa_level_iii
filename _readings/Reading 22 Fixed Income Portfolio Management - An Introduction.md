---
sequence: 22
title: 'Reading 22: Fixed Income Portfolio Management - An Introduction'
section: 9
sectionTitle: 'Fixed Income Portfolio Management'
firstReading: true
layout: reading
---

# Reading 22: Fixed Income Portfolio Management - An Introduction

## 22.A: Discuss roles of fixed-income securities in portfolios

- Fixed income has many roles within a portfolio:
  - Due to low correlation with equity assets, fixed income provides diversification benefits
    - US-based investment grade (IG) fixed income assets are usually well correlated with each other
    - Emerging market (EM) and high-yield (HY) fixed income offers low correlation to IG assets, but high correlation with equities
    - These general facts however are not always stable, for example, when investors seek safe havens in times of crisis, higher risk assets fall together, with correlation approaching 1
  - Regular cash flows
  - Inflation-linked and floating rate bonds can function as an inflation hedge

## 22.B: Describe how fixed-income mandates may be classified and compare featurs of the mandates

- A portfolio managed with the sole intention of meeting obligations of future payouts is a **liability-based mandate**
  - Arranging assets in this way is referred to as immunisation, of which there are multiple types:
    - **Cash-flow matching** arranges the cash flows from assets so they provide the cash flows due on other liabilities
    - **Duration matching** ensures that both assets and liabilities will change in the same manner as interest rates change, ensuring that assets still cover liabilities
    - **Contingent immunisation** involves building a portfolio with an initial surplus over liabilities, and managing it with the goal of increasing the surplus
      - If successful, this approach may end up cheaper than others, due to the increased surplus
      - If not, the portfolio must realign to a new means of immunisation, and the capital used to build the initial surplus is wasted
    - **Horizon matching** is a hybrid approach that utilised cash-flow matching for short-term liabilities, and duration matching for long-term liabilities
      - Since duration matching offers a less restrictive pool of assets to choose from, it can be done more cheaply than pure cash-flow matching

- **Total return mandates** have a goal of generating return instead of covering some liability
  - **Pure indexing** aims for no additional return above that of a benchmark, seeking merely to replicate the index
    - This does allow some leeway in individual securities selected, whilst matching factor exposures, and targeting no active return or active risk
  - **Enhanced indexing** targets some level of restrained seeking of alpha (around 30 bps), mostly still duration matched with some deviation
  - **Active management** seeks even higher levels of alpha, above 50 bps

## 22.C: Describe the bond market liquidity, including the differences among market sub-sectors, and discuss the effect of liquidity on fixed-income portfolio management

- Whilst recently issued bonds may be very liquid, others may be highly illiquid, leading to large bid-ask spreads, or indeed never trading at all
  - Since there are large numbers of small bond issues, each with different maturieis, features, and yields, trade volume for an individual issue can be small compared to common stock for a publicly traded firm
  - Bond trades are generally over the counter, increasing the cost of transactions, and reducing transparency

- Soverign debt that is high quality and recently issued can be highly liquid
  - Corporate bonds are far more varied, although liquidity tends to decrease with:
    - Increased risk
    - Reduced size of issue
    - Increased age of issue

- Whilst in some markets bond pricing information is centralised, this is not always the case, and in some circumstances accurate pricing information is difficult to find
  - Additionally, since the information available may be out of date for rarely traded bonds, **matrix pricing** is used
    - Matrix pricing involved determining an implied price by collating data on similar bonds that have been more recently traded, using the YTM of each
      - Additional features of an issue can make bonds less comparable

- Investors with lower liquidity needs may actually seek bonds that are less frequently traded in order to earn a liquidity premium

- There are alternatives to fixed income investment available as derivatives
  - Bond futures and options, are exchange traded, whilst interest-rate swaps and credit default swaps are available over the counter
    - In some jurisdictions however, derivatives trading entails abiding by other regulations
  - ETFs that replicate features of fixed-income investment provide a more liquid alternative that may be attractive to some investors

## 22.D: Describe and interpret a model for fixed-income returns

- Return from fixed income has five main parts:
  - **Income yield**
    - This component is the annual coupon income divided by the price of the bond
    - Note that neither of these inputs are projections, and use actual known amounts
  - **Rolldown return**
    - This component emerges from a projection of a bond's future prices assuming the yield curve remains fixed
  - **Expected price change**
    - Calculated from expected change in spreads and yield using the following:
$$\Delta \text{PV}=(-\text{modifed duration} \cdot \Delta Y)+(\frac{C}{2} \cdot \Delta Y^2)$$
    - $C$ denotes convexity, which adds an adjustment to the relationship between changes in price and changes in yield
      - As yields go up, prices go down, but due to convexity the strength of this relationship weakens for greater changes in yield
  - **Credit losses**
    - Simply, the probability of default multiplied by the amount loss in the event of default
  - **Gains or losses vs. investor currency**
    - Calculated as $R_\text{FC} \cdot \text{\% invested in foreign currency}$

## 22.E: Discuss the use of leverage, alternative methods for leveraging, and risks that leverage creates in fixed income portfolios

- As long as the interest onborrowed funds is below rates of return, leverage enhances return overall
  - However, it also increases exposure to interest rate risk
  - Since leverage normally utilises short term financing, asset duration usually exceeds that of liabilities

- Repurchase agreements is an agreement to sell an asset for cash, and also to buy it back on a future date
  - The asset effectively functions as collateral on the loan
  - Terms are usually short, on the order of a day, but they can be renegotiated at expiry, as well as agreed for longer terms
  - Typically the assets transferred are not specified, and instead take the form of "general collateral"
  - Rather than adjusting the repo rate for the quality of collateral, the amount of collateral required is adjusted, with lower quality collateral entailing a larger *haircut*
    - The haircut is the additional collateral required to provide additional security, beyond matching the value of the loan
    - The haircut will be larger if the underlying asset is more volatile
  - Repos can be bilateral aggreements between lender and borrower, or tri-party, with an intermediary managing the exchange and holding the collateral
    - This can often be less expensive than arranging an actual exchange of collateral
  - A security driven repo involves a lender with a temporary need for a specific security, possibly for hedging reasons, and may offer a lower repo rate in return for that specific asset being delivered as collateral

- **Futures contracts** require only a small initial deposit to provide leverage
  - The price of the contract gives the value of the asset controlled via a multiplier

- **Swap agreements** can also provide leverage
  - A receive-fixed swap provides fixed-income exposure and interest rate exposure
  - Before the financial crisis entering a swap was reasonably unregulated and did not require collateral
  - Since the crisis many swaps are settled via a clearinghouse

- **Securities lending** often facilitates short-selling, allowing investors to sell assets they do not own by borrowing them
  - The lender of the securities may require cash in return, and invest it until the security is returned
  - Alternatively the lender may receive another securitiy, such as a government bond, earning interest on the collateral whilst they hold it
  - If the interest on the collateral exceeds a fair price for the security, the borrower posting the collateral may receive a rebate
  - These agreements typically persist until one counterparty requires that it is closed (as distinct from repo agreements
    - This can possibly lead to counterparty risk

- Leverage creates the risk of **fire sales**, which occur when rapid liquidations and selling occur within crisis
  - If the cost of leverage exceeds returns, lenders may demand repayment within a short time frame
  - This can lead to a vicious cycle where prices everywhere fall, further exacerbating the situation

## 22.F: Discuss differences in managing fixed income portfolios for taxable and tax exempt investors

- Fixed income investing usually produces two kinds of income, interest and capital gains, that may be taxed differently
  - Both are usually taxable only when realised, but there are some exceptions
    - For example, on zero coupon bonds, the approaching of the price towards par may be taxed annually, despite the lack of cash flows
  - Capital gains taxes are usually only due upon sale, and at a lower rate than interest
    - The rate may be higher if the assets are only held for a short period
  - Capital gains (and only capital gains) can be offset by capital losses
    - If losses exceed gains they can be carried forward

- Taxation of funds varies by jurisdiction
  - Interest and dividends are usually taxed when earned, not when distributed
  - Some jurisdictions use **pass through taxation of gains** taxes investors in the fund when the gain is realised by the fund, reducing the tax payable by the investor when they sell a share in the fund
  - Others simply tax investors when they sell shares in the fund