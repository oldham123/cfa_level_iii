# Reading 11: Taxes and Private Wealth Management in a Global Context

## 11.A: Compare basic global taxation regimes as they relate to the taxation of dividend income, interest income, realised capital gains, and unrealised capital gains

- Taxes come in three general forms:
  - Taxes on income
  - Taxes on consumption
  - Taxes on wealth
- Taxes are used to:
  - Raise revenue
  - Shape behaviour
- Taxes can be flat, where the same percentage is applied to all, or progressive, where the percentage increases with income
  - The *marginal tax rate* is the highest rate at which someone is assessed
  - Progressive tax systems usually contain a series of *income brackets*, where income falling within each bracket is taxed at a different rate. For example, consider an individual income of $173,000 if:
    - The first $8,350 of income is taxed at 10%
    - Additional income up to $33,950 is taxed at 15%
    - Additional income up to £82,250 is taxed at 25%
    - Additional income up to $171,550 is taxed at 28%
    - Additional income up to £373,950 is taxed at 33%
    - Any additional income is taxed at 35%
  - In this example, the marginal tax rate is 33%
  - The average tax rate is $\approx$ 24.4%
  - Total taxes due is $42,232.50
- Different forms of income may also be taxed at different rates, including interest, dividends, or capital gains
  - They may also be taxed differently based on whether they are accrued over the long term or short term
  - The most common tax regime seen globally is *common progressive*, which features progressive income taxes, as well as favourable treatment of interest, dividend, and capital gains income
  - The second most common is the same, except there is less favourable treatment of interest and dividend income

## 11.B: Determine the effects of different types of taxes and tax regimes on future wealth accumulation

## 11.C: Explain how investment return and investment horizon affect the tax impact associated with an investment

- The impact of taxation on returns is non-trivial, and it varies greatly
- *Accrual taxes* are usually annual taxes applied at a single rate on a single category of income
  - Interest and dividends are usually treated this way
  - The future value of an investment after accrual taxes is given by:

$$
FVIF = \Big( 1 + r \cdot (1 - t_i) \Big)^n
$$

- One way to express the impact of taxes on an investment is by calculating *tax drag*, expressed either as a percentage, or an absolute value:

$$
\begin{aligned}
\text{tax drag}_\$ &= \text{gain lost}\\
&=\text{gain with no tax} - \text{gain after tax}\\
&=\text{FV}_\text{PT} - \text{FV}_\text{AT}\\
\\
\text{tax drag}_\% &= \% \text{ gain lost}\\
&=\frac{\text{tax drag}_\$}{\text{FV}_\text{PT} - \text{PV}}
\end{aligned}
$$

- Tax drag has several important features:
  - Where $n > 1$,  the drag percentage is greater than the tax rate
  - The drag percentage increases as the time horizon increases
  - The drag percentage increases as the rate of return increases
- Taxes on capital gains are only incurred when the asset is sold, and only on the gain in value of the asset
  - Since the time of sale is controlled by the owner of the asset, the timing of the tax can be controlled
  - This deferment of tax removes the compounding effects of tax drag, such that tax drag is constant as time horizon varies
  - If $B​$ is the tax cost basis of the asset, then the future value is given by:

$$
\text{FV}_\text{AT} = (1+r)^n \cdot (1 - t_\text{cg}) + t_\text{cg} \cdot B
$$

- The first component of this formula calculates the future value as if the entire asset value were taxable
  - The second component adds back in the tax on the original value, since taxes are only due on the gains
- Wealth taxes are imposed on *total value*, as opposed to returns
  - Future value under wealth taxation is given by:
$$
\text{FV}_\text{AT} = \Big( (1+r) \cdot (1 - t_w) \Big)^n
$$
  - The following is generally true for annual wealth taxes:
    - Wealth taxes are larger than other forms of tax
    - Tax drag increases with time horizon
    - Tax drag decreases with return
      - This is because tax drag is a function of the gain, whilst the tax itself is also a function of the original value, which remains fixed as return increases
- Multiple taxation methods are usually applicable to a portfolio
  - A portfolio can generate returns from interest, dividends, as well as capital gains, with each potentially subject to a different tax rate
  - Weighted average realised tax rate can be calculated using the proportion of total return each type contributes, and the tax rate on each
$$
\text{WARTR} = p_\text{i} \cdot t_\text{i} + p_\text{d} \cdot t_\text{d} + p_\text{cg} \cdot t_\text{cg}
$$
  - The return after taking realised taxes into account is given by the following:
$$
r_\text{ART} = r_\text{PT} \cdot (1 - \text{WARTR})
$$
  - It is important to note that $r_\text{ART}$ overstates after-tax return, since it does not take into account the deferred taxes due to not yet realising all of the capital gains
  - Calculating the final after-tax return can be projected by calculating an effective capital gains tax rate given by:
$$
\begin{aligned}
\text{T}^* &= t_\text{cg} \cdot \Bigg[ \frac{1 - (p_\text{i} + p_\text{d} + p_\text{cg})}{1 - (p_\text{i} \cdot t_\text{i} + p_\text{d} \cdot t_\text{d} + p_\text{cg} \cdot t_\text{cg})} \Bigg]\\
&=t_\text{cg} \cdot \Big[ \frac{p_\text{dcg}}{1 - \text{WARTR}} \Big]
\end{aligned}
$$
  - This can then be applied to a modified calculation for future value after capital gains:
$$
\text{FV}_\text{AT} = (1 + r_\text{ART})^n \cdot (1 - T^*) + T^* - (1 - B) \cdot t_\text{cg}
$$

  - Once all tax effects are accounted for, an **accrual equivalent return** can be calculated:
$$
\text{R}_\text{AE} = \Big( \frac{\text{FV}_\text{AT}}{\text{initial investment}} \Big)^{\frac{1}{n}} - 1
$$
  - The equivalent tax rate is calculated using:
$$
\text{T}_\text{AE} = 1 - \frac{\text{R}_\text{AE}}{r}
$$