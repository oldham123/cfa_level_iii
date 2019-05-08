---
sequence: 33
title: 'Reading 33: Risk Management Applications of Option Strategies'
section: 13
sectionTitle: 'Risk Management Applications of Derivatives'
layout: reading
---

# Reading 33: Risk Management Applications of Option Strategies

## Secret Sauce Notes

- For strategies using options, it is important to understand the payoff patterns that result from option combinations
  - This involves understanding the return generated at various final prices for the underlying
  - Sum the ending option value with returns or losses on the initial investment

- A **covered call** strategy combines an underlying security, with selling a call option
  - If the price of the underlying rises above the option strike price, the buyer of the investor's call will exercise, limiting upside
  - The downside potential is retained
  - Option premium income is generated
  - Usually ideal for stable assets

- A **protective put** strategy combines an underlying security, with buying a put option
  - If the price of the underlying falls below the option strike price, the investor can exercise, limiting downside
  - The upside potential is retained
  - Option premium must be paid
  - Usually ideal for volatile assets

- A **bull spread** strategy combined a long call at a low strike price, and a short call at a high strike price
  - Alternatively a short put at a high strike price, and a long put at a low strike price have the same effect
  - If the price of the underlying rises above the strike price, the buyer of the call will exercise, which limits upside
    - Alternatively, both puts expire, worthless, with a limited upside equal to the net premium
  - If the price of the underlying falls below the strike price, then both options are exercised, with downside limited to the difference between strike prices, minus the option premium income

- A **bear spread** strategy combines a long put at a high strike price, and a short put at a low strike price
  - Alternatively a short call at a low strike price, and a long call at a high strike price
  - If the price of the underlying rises above the strike price, both options expire worthless, with a loss equal to the option premiums paid
    - Alternatively, both calls are exercised, with a loss equal to the difference between strike prices, plus option premiums
  - If the price of the underlying falls below the strike price, both options are exercised, leading to a profit equal to the difference between strike prices, minus the option premiums paid

- A **butterfly spread** strategy combines four options at three different strike prices, and gains if the underlying is stable, composed of:
  - Long calls at a high and low strike price, and two short calls at a medium price
  - The same but with puts
  - A short put and call at a medium strike price, a long put at a low strike price, and a long call at a high strike price

- A **straddle** combines a long put and call at the same strike price to gain from volatility
  - A reverse straddle is the same but shorts the options to gain from decreasing volatility

- A **collar** is similar to a bull spread
  - It combines a long put at a low strike price, a short call at a high strike price, as well as the underlying

- A **box spread** combines  bull and bear spread
  - Assuming options are priced fairly, it will yield the risk-free rate

- **Interest rate options** are usually based on LIBOR
  - The call receives the underlying rate, and pays the strike rate, whilst the put receives the strike rate and pays the underlying rate
  - An **interest rate cap** is a series of interest rate calls, which compensates the buyer for rising interest rates, effectively keeping them fixed
    - Each constituent call is called a **caplet**
    - The inverse can be achieved with series of puts, creating a **floor**, which each put called a **floorlet**
  - Combining a short cap with a long floor creates an interest rate collar

- **Delta hedging** is a strategy that earns the risk-free rate by taking equal and opposite positions in an option, and the underlying asset
  - The number of shares $\#_\text{shares}$ required to perfectly hedge a given number of options $\#_\text{options}$ is given by $\Delta_\text{option} \cdot \#_\text{options}$
  - **True delta** is the change in option value given a change in value of the underlying
    - It is the $N(d_1)$ term from the Blak-Scholes-Merton formula
    - $\Delta_\text{option} \approx \frac{\Delta V_\text{option}}{\Delta V_\text{share}}$
    - Similarly, **gamma** is the change in delta given a change in value of the underlying