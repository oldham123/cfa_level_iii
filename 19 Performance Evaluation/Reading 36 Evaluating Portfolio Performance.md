# Reading 36: Evaluating Portfolio Performance

## Secret Sauce Notes

- Return on an asset with external cash flows depends on when those cash flows are generated
  - Where the value of an asset changes from $V_\text{initial}$ to $V_\text{final}$, providing a cash flow at the start of the evaluated period of $\text{CF}_1$ and another cash flow at the end of the period $\text{CF}_2$, return $r$ is given by:
$$
r = \frac{(V_\text{final} - \text{CF}_2) - (V_\text{initial} + \text{CF}_1)}{V_\text{initial} + \text{CF}_1}
$$

- Return can generally be attributed to three main sources
  - Return $P$ is made up of *market return* $M$, *style return* $S$, and *active management return* $A$:
$$
P = M + S + A
$$
  - Active management decisions represent the difference between portfolio and *benchmark return* $B$:
$$
P = B + A
$$
  - The difference between benchmark return, and return on a generic *market index* $M$ represents return due to *style*:
$$
S = B - M
$$

- A valid benchmark should have the following seven attributes:
  - Pre-specified
  - Appropriate
  - Measurable
  - Unambiguous
  - Reflective of current investment opinions
  - Accountable
  - Investable

- There are seven main types of benchmark available:
  - Absolute
  - Manager universes
  - Broad market indices
  - Style indices
  - Factor-model-based
  - Returns-based
  - Custom security-based
    - These are constructed by:
      - Identify the manager's investment process, asset selection, and weighting
      - Use the same assets and weights for the benchmark
      - Rebalance at pre-determined intervals

- Benchmark quality can be tested in the following ways:
  - Check that systematic bias relative to the account is minimal
  - Check that active management returns and style returns are uncorrelations
  - Check that tracking error is minimal
  - check that an accounts systematic risk is similar to the benchmark
  - Check that the coverage ratio is high
  - Check that passive accounts use benchmarks with low turnover
  - For active long-only accounts, the benchmark should primarily involve positive active positions

- When attributing performance to various factors, it is done at two mains levels:
  - **Macro performance** is attributed to *fund sponsors*, and involves:
    - Policy allocations
    - Benchmark returns
    - Fund returns, valuations, and cash flows
  - **Micro performance** is attributed to *fund managers* and can be done at any of the following levels:
    - Net contributions
      - This is how managers allocate proportions of total assets to each level of the fund, placing assets into a higher level only if the level below will generate sufficient return
    - Risk-free assets
    - Asset categories
      - This involves the decisions of fund allocation between various category benchmarks, as part of benchmark replication
    - Benchmarks
      - At this level funds are passively managed, but allocations into manager *style benchmarks*
    - Investment managers
    - Allocation effects

- **Value-added return** can be used to perform micro-performance attribution, and it features three main components, which can be summed together:
  - Return due to sector allocation:
$$
\sum^S_{i = 1} (w_\text{P,i} - w_\text{B,i}) \cdot (R_\text{B,i} - R_\text{B})
$$
  - Return due to allocation interaction:
$$
\sum^S_{i = 1} (w_\text{P,i} - w_\text{B,i}) \cdot (R_\text{P,i} - R_\text{B,i})
$$
  - Return due to allocation within sectors:
$$
\sum^S_{i = 1} w_\text{B,i} \cdot (R_\text{P,i} - R_\text{B,i})
$$
  - The strengths of this method include:
    - The ability to disaggregate the impact of sector, and security decisions
    - Ease of calculation
  - Limitations include:
    - The importance of selecting an appropriate benchmark
    - The relationship between security selection and sector weighting can effect the disaggregation

- Another way of attributing performance is through the use of a fundamental factor model
  - Combining sector fectors with other fundamentals requires:
    - Identifying the factors that generate systematic returns
    - Determining portfolio and benchmark exposures to the chosen factors
    - Specifying a benchmark set of exposures, such as those of an index
    - Determining the performance of each factor
  - Strengths of this method include:
    - Attribution of performance to actual factors instead of just weightings
  - Limitations include:
    - Factor exposures must be determined
    - Mathmematically complex, possibly leading to spurious correlations

- Fixed-Income performance can be thought of as being composed of the following:
  - Success in predicting interest rate movements
  - Success in over or under weighting various sectors
  - Success in selection superior securities
  - Residual performance thought of as representing returns to successful active trading

- Risk-adjusted performance measures include:
  - **Ex-post alpha**
    - Uses the security market line as an appraisal benchmark
$$
\alpha_p = R_p - \left[R_F + \beta_p \cdot (R_m - R_F)\right]
$$
  - The **Treynor Measure** compares active return against *beta*
  - The **Sharpe Ratio** compares active return against *total risk*
  - The **$M^2$ Measure** uses the capital market line, and the Sharpe ratio to compare portfolio performance to that of the market:
$$
M^2_P = R_F + \left( \frac{R_P - R_F}{\sigma_P} \right) \cdot \sigma_M
$$

- Quality control charts can illustrate whether a portfolio is performing according to expectations with respect to a chosen benchmark
  - Value-added return is plotted over time, alongside the upper and lower bounds of the 95% confidence interval of expectations
  - In order to plot the chart, and analyst needs:
    - A null hypothesis (usually that value-added return is zero)
    - Independent and normally-distributed value-added returns
    - Effectively constant variance of value-added returns

- **Manager Continuation Policies** are subject to the following guidelines:
  - Only replace managers when justified
  - Formal policies should be created and applied consistently to all managers
  - Managers should be assessed using reasonable performance measurement and attribution techniques, as well as:
    - The usage of appropriate strategies
    - The selection of appropriate benchmarks
    - Account growth

- **Errors** can be divided into **Type I** and **Type II**
  - Given a null hypothesis that managers are not adding value, and an alternative hypothesis that they are
    - A Type I error would be the retention of a manager that adds no value
      - i.e. *Failing to reject when appropriate*
    - A Type II error would be the replacement of a manager that does add value
      - i.e. *Rejecting when inappropriate*