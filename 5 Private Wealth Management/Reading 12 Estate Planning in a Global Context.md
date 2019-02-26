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

## 12.F: Evaluate the after-tax benefits of basic estate planning strategies, including generation skipping, spousal exemptions, valuation discounts, and charitable gifts

- If an investor hopes to gift assets to a grandchild, this could potentially incur double taxation (once in the transfer to the child, and again in transfer to *their* child)
  - **Generation-skipping transfer taxes** are incurred to prevent direct transfers to grandchildren being used to prevent this double taxation
  - In some jurisdictions however, such as the USA, these taxes do not exist, and hence this remains an efficient strategy
  - If skipping generations is possible, the value of the gift increases by $\frac{1}{1-t_g}$
    - This is the **relative value of generation skipping**
  - The appropriate amount to transfer can be determined by subtracting core capital requirements for the first and second generations from the total estate
- Many tax regimes also allow tax-free transfers between spouses, although whether the use of them is efficient from a tax perspective depends on other factors
  - For example, if there is an amount that can be transferred directly to children tax-free, it would instead be optimal to take advantage of that first, and only transfer the rest to the spouse

- Ownership claims in private entities are difficult to value, and often lead to **valuation discounts**
  - These discounts can cause the value of an estate to effectively fall, leading to greater tax efficiency
  - The claim in the private entity is calculated by making use of comparables, and then applying a discount for illiquidity, and a lack of control
  - It is important to note that these discounts are subject to court approval, and often reduce as the size of firm increases

- When the investor wants to make a gift to a tax-exempt charity, the ratio used to determine whether to gift now, or bequeath, is again altered
  - The numerator is given by the tax-free return that the charity can earn on the gift, as well as the tax saving of $T_{oi}$ for each dollar gifted, which can be invested by the donor, generating a return $r_e$, taxed at $t_{ie}$, and then taxed at death upon transfer at $T_e$
$$
\frac{(1 + r_g)^n + T_{oi} \cdot \Big( 1 + r_e \cdot (1 - t_{ie}) \Big)^n \cdot (1 - T_e)}{\Big(1 + r_e \cdot (1 - t_{ie})\Big)^n \cdot (1 - T_e)}
$$

## 12.G: Explain the basic structure of a trust and discuss the differences between recovable and irrevocable trusts

- A **grantor** may place funds into a **trust** as a means of transferring funds without going through probate
  - The trust is managed by a **trustee**, who manages the assets on behalf of the beneficiaries, and according to constraints set by the grantor
  - The legal owner, as well as the owner for tax purposes, may be either the trustee or the grantor, depending on the circumstances
- Trusts can be either revocable, or irrevocable
  - The grantor remains the owner of the assets in the case of **revocable trusts**, has the power to revoke the trust, and trust creditors retain the ability to make claims against trust assets
  - The grantor gives up control of the assets in an **irrevocable trust**, and instead the trustee is considered the owner, in which case claims cannot be made against assets
    - If the trust was made with the intent of nullifying a claim, then these claims remain valid
- There are two main kinds of trust:
  - A **fixed trust** entails predetermined distributions of assets codified within trust documents
  - A **discretionary trust** empowers the trustee to make decisions regarding asset distribution, and beneficiaries have no automatic right to the assets
- A **spendthrift trust** is a means of transferring assets to individuals unable to manage them, either due to age, or some other circumstance
- In some countries, regardless of the type of trust, the grantor remains responsible for taxes on the trust, remaining the owner for tax purposes
- Trusts are more abundant in common law countries, whilst foundations are more abundant in civil law countries

## 12.H: Explain how life insurance can be a tax-efficient means of wealth transfer

- Funds paid out from life insurance policies do not incur taxes in most jurisdictions, and hence they are often an efficient means of transferring wealth
  - In addition, trusts can be established as the beneficiary of a life insurance policy

## 12.I: Discuss the two principal systems (source jurisdiction and residence jurisdiction) for establishing a country's tax jurisdiction

## 12.J: Discuss the probable income and estate tax consequences of foreign situated assets and foreign-sourced income

- **Source jurisdiction**: All income generated within its borders is taxed, no matter by whom it is generated
- **Residence jurisdiction**: All income generated by a country's citizens is taxed by that country, regardless of where it is generated
  - Tests to determine residence vary significantly

- Wealth transfers are taxed are treated differently under each:
  - Under source jurisdiction, taxes are paid on transfers occuring within the country, regardless of who makes them
  - Under residence jurisdiction, transfer taxes are paid both by citizens and residents, regardless of location

- **Exit taxes** are taxes incurred upon renouncing citizenship, often based on gains on assets being taken
  - It may also include income taxes incurred during a **shadow period** following expatriation

## 12.K: Evaluate a client's tax liability under each of three basic methods (credit, exemption, and deduction) that a country may use to provide relief from double taxation

- If two countries use means of determining residence that lead them to conclude that the individual is resident in both nations, this may result in that individual being liable to pay taxes on the same assets or income twice
  - This is known as **residence-residence conflict** and can lead to **double taxation**
  - Additionally, **source-source conflict** is also possible, possibly leading to the same result
    - Consider an MNC with revenue generating activity occuring within multiple jurisdictions
  - **Residence-source conflict** occurs when an individual is deemed a resident of one jurisdiction, whilst generating income or transferring wealth in another
- Some nations have devised ways of helping individuals avoid double taxation
  - The **exemption method** allows individuals to be completely exempt from tax in the residence country after paying tax to the source country
  - The **credit method** nets off taxes paid to the source country against taxes owed to the residence country
    - If an individual owes $100 to the residence country and $80 to the source country, the amount owed to the residence country would reduce to $20
  - The **deduction method** allows taxes paid to the source country to be *deducted* from taxable income before taxes are paid to the residence country

## 12.L: Discuss how increasing international transparency and information exchange among tax authorities affect international estate planning

- The aim of financial planners is to structure estates in the most tax-efficient ways
  - This may involve offshoring assets
- The distinction between legal and illegal activity is of vital importance in estate planning:
  - **Tax avoidance** is the legal arranging of affairs in order to reduce the amount of tax owed
  - **Tax evasion** involves dishonest activity to *illegally* avoid taxation
- Estate planners should arrange assets as efficiently, and as legally as possible, so as to avoid legal complications arising from the use of tactics not covered by global tax agreements between regimes
- Most countries attempt to collect as much revenue as possible, and enter into global treaties which allow for the sharing of information between tax authorities
  - For example, the IRS requires that the names of the owners of US securities are disclosed to them, regardless of that person's citizenship
  - As a result, many banks have become **qualified intermediaries**only provide information on US customers
  - A similar situation exists in the EU