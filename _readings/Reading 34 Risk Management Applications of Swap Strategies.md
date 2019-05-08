---
sequence: 34
title: 'Reading 34: Risk Management Applications of Swap Strategies'
section: 13
sectionTitle: 'Risk Management Applications of Derivatives'
layout: reading
---

# Reading 34: Risk Management Applications of Swap Strategies

## Secret Sauce Notes

- Swaps can be used to convert floating liabilities into fixed liabilities, and vice versa
  - Combining a floating rate liability with a pay fixed receive floating swap results in a fixed rate liability
  - Combined a fixed rate liability with a pay floating receive fixed swap results in a floating rate liability

- Fixed rate liabilities may have high absolute duration whilst floating rate liabilities may have low absolute duration
  - Duration of a floating rate security is usually approximated as $\frac{1}{2}$ the reset period
  - Duration of a zero coupon bond is simply the maturity
  - For non-zero coupon bonds, duration increases with maturity, but is slightly less, since the weighted average date upon which cash flows are received is brought forward by coupon payments

- Since the cash flows of an interest rate swap can be replicated by combining pay fixed and pay floating instruments, duration can be calculated in a similar way
  - The duration of a pay floating swap, is the duration of a fixed-rate bond, minus the duration of a floating-rate bond
  - The duration of a pay fixed swap is the duration ofa floating-rate bond, minus the duration of a fixed-rate bond

- Given a swap with modified duration $\text{MD}_\text{swap}$, and a portfolio of current duration $\text{MD}_\text{P}$ and value $V_\text{P}$, and a desired duration $\text{MD}_\text{T}$, the required number of swaps is given by:
$$
\text{NP} = V_P \cdot \left( \frac{\text{MD}_\text{T} - \text{MD}_\text{P}}{\text{MD}_\text{swap}} \right)
$$

- A **currency swap** involves an exchange of notional principals upon initiation, in return for which each party makes coupon payments
  - At termination, the notional principals are returned
  - This means that a firm that needs to borrow one currency, but can achieve favourable rates for another currency, can benefit from a swap
    - The cheaper financing currency is borrowed, and then exchanged in return for the desired currency
    - The investor then makes coupon payments in the desired currency, and in return receives coupon payments in the financing currency
  - A special form of currency swaps neglects the transfer of the initial principals in order to convert streams of payments in one currency to payments in another

- **Equity swaps** allow investors to provide the return on one position to receive the return on another
  - This allows investors to, for example, py the return on a concentrated stock position in return for receiving the return on a diversified index
  - Alternatively, an investor could effectively convert the return on one index into the return on another

- A **swaption** is an option to initiate  pre-negotiated swap
  - The naming convention refers to whether the long received or pays the fixed side