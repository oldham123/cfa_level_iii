# Reading 12: Estate Planning in a Global Context

## 12.A Discuss the purpose of estate planning and explain the basic concepts of domestic estate planning, including estates, wills, and probate

- An investor's **estate** is the sum total of everything owned by that investor
  - The process of arranging for the transfer of one's estate to others (either before or after death) is **estate planning**
  - A **will** is a document that establishes the legal rights that others may have to an investor's estate after their death
  - The **testator** is the individual using the will to move assets

- Upon an investor's death, the validity of a will is determined by a court, and the assets are distributed accordingly, in a process called **probate**
  - Costs associated with probate are taken from the estate
  - In the absence of a valid will, and investor has died **intestate**, and a court determines the distribution

- Since probate is costly, investors may attempt to avoid it by organsing transfer before death, through things such as *shared ownership*, *living trusts*, *retirement plans*, and so on

- Investments in private companies can be an efficient form of estate planning, since the uncertainty of true value, as well as a lack of liquidity and control lead to valuation discounts

## 12.B Explain the two principal forms of wealth transfer taxes and discuss effects of important non-tax issues, such as legal system, forced heirship, and marital property regime

- Assets can be transfers using **gifts** or **bequests**:
  - Gifts may be subject to taxes, depending on the relevant jurisdiction
  - Bequests may also result in **estate taxes** (paid by the giver) or **inheritance taxes** (paid by the receiver)
  - The treatment of these transfers can vary greatly depending on the specific circumstances

- Many of the geographical differences between tax treatments are due to the foundations of legal systems
  - **Civil law** systems involve legislative bodies that pass laws down
  - **Common law** systems give judges the role of interpreting laws and laying down precedent, effectively creating law from the bottom up

- Different tax regimes can operate different definitions of even concepts as basic as ownership
  - **Forced heirship** guarantees the right of a child to their parent's estate, regardless of the situation that exists between them
  - Investors may attempt to avoid forced heirship by moving their estates into another jurisdiction
  - **Clawback** provisions have been established in retaliation that only calculate a child's share of an estate after those transferred sums are added back
  - If there is an amount withstanding the child may have legal recourse to claim any remaining funds from the current owners

- **Marital property rights** are rights to an estate possessed by a spouse, a specific form of forced heirship
  - A **community property rights** tax regime entitles a spouse to half of anything gained during the marriage
  - Certain items such as gifts of inheritance may be held separately
  - A **separate property rights** regime grants each spouse control over to whom assets may be distributed after death

## 12.C: Determine a family's core capital and excess capital, based on mortality probabilities and Monte Carlo analysis

- An individual can be thought of as owning assets equal to the value of any actual assets currently owned, plus additional **human capital**, or **net employment capital** the present value of income from employment likely to be earned
  - Liabilities can be thought of as the present values of all costs likely to be incurred
    - Some of these are literal liabilities, such as debts, as well as funds required to sustain a current standard of living
  - Netting these off against each other yield's an individuals **excess capital**
- **Core capital** is the capital required to settle all liabilities, plus an emergency reserve, with excess capital being any amount above this
- **Mortality tables** are a statistical tool used to determine an individuals *expected remaining years*
  - They are constructed using average life expectancy, and hence if they are used to determine core capital, and an investor matches this figure with no excess, there is a 50% chance that they will outlive their core capital
    - Hence, a **safety reserve** to top up the core capital and provide some excess may be advisable
    - Additionally, this method assumes a steady risk-free rate of return on assets
    - Furthermore, failing to predict spending patterns creates path dependency risk, possibly resulting in drawing down available funds too early, and making the required returns unattainable
    - A mortality table is used by first adjusting each future year's expected spending by the probability of living to that year, and then discounting it to the present day

- Monte Carlo simulation is a valuable tool in retirement planning, allowing the specification of probability distributions of multiple variables
  - These are then used to simulate a scenario many thousands of times, obtaining a distribution of outcomes with various likelihoods of occuring
  - The model can then inform sensible adjustments to the plan early on, helping to avoid bad scenarios
  - One use is to determine a required amount of core capital, by adjusting initial capital inputs, and observing how long they last in various scenarios
  - The model also accounts for path dependency, with each simulation modelling precisely a pattern of withdrawals and deposits
  - A further benefit is enabling the calculation of a **probability of ruin** (of the portfolio reaching zero value), also according to various input values, such as the starting date of retirement

## 12.D: Evaluate the relative after-tax value of lifetime gifts and testamentry bequests

## 12.E: Explain the estate planning benefit of making lifetime gifts when gift taxes are paid by the donor, rather than the recipient

- Wealthy investors face the choice of gifting capital when alive, or bequesting it after death
  - Gifts entail losing control of capital immediately
  - Gifts and bequests can entail different tax treatments
- One approach is to calculate a ratio from the perspective of the recipient given by:

$$
\frac{\text{FV}_\text{AT gift}}{\text{FV}_\text{AT bequest}}
$$

- When gifting capital, the amount can either:
  - Be tax-exempt
  - Incur taxes upon the donor
  - Incur taxes upon the recipient
- A ratio that aids in this analysis can be determined by considering the following factors:
  - $r_g$ and $t_{ig}$, the pre-tax return and tax rate associated with the amount gifted
  - $r_e$ and $t_{ie}$, the pre-tax return and tax rate associated with the amount retained within the estate
  - $T_e$, the tax incurred on the estate upon transfer
  - $T_g$, the tax incurred on the gift upon transfer
  - $p_g$ and $p_e$, the proportions of capital gifted and retained in the estate respectively

- In the event that gifts are tax exempt, the value after tax if gifted is simply the return generated on the amount, with the relevant tax rate applied to the returns, compounded over expected years till death:
$$
\frac{\Big(1 + r_g \cdot (1 - t_{ig})\Big)^n}{\Big(1 + r_e \cdot (1 - t_{ie})\Big)^n \cdot (1 - T_e)}
$$

- If the recipient of the gift incurs a tax on the funds, the value after tax if gifted is a similar calculation, also accounting for the tax applied to the gift:
$$
\frac{(1 - T_g) \cdot \Big(1 + r_g \cdot (1 - t_{ig})\Big)^n}{\Big(1 + r_e \cdot (1 - t_{ie})\Big)^n \cdot (1 - T_e)}
$$

- If the donor incurs a tax on the funds, this tax will reduce the value of the estate (contingent on the proportions gifted and retained), and thus the value of taxes incurred on the estate, essentially functioning as a tax credit:
$$
\frac{(1 - T_g + T_g \cdot T_e \cdot \frac{g}{e}) \cdot \Big(1 + r_g \cdot (1 - t_{ig})\Big)^n}{\Big(1 + r_e \cdot (1 - t_{ie})\Big)^n \cdot (1 - T_e)}
$$

- Charitable gifts of appreciated securities allow the investor in many cases to avoid gift transfer taxes, by taking an income tax deducation that equals the gift's current market value
  - Once transferred to a tax exempt organisation, capital gains taxes continue to be avoided