---
sequence: 32
title: 'Reading 32: Risk Management Applications of Forward and Futures Strategies'
section: 13
sectionTitle: 'Risk Management Applications of Derivatives'
firstReading: true
layout: reading
---

# Reading 32: Risk Management Applications of Forward and Futures Strategies

## Secret Sauce Notes

- Derivates can be used to adjust portfolio exposures
  - Buying equity contracts increases equity exposure, and portfolio beta
  - Buying bond contracts increases bond exposure, and portfolio duration
  - The inverse can be achieves by selling them
  - The number to buy or sell is determined by the desired shift in exposure
  - Where $T$ denotes target, $P$ denotes portfolio, $f$ denotes future, $P$ denotes price, $\beta$ denotes beta, $\text{MD}$ denotes duration, and $V$ denotes value, the number of contracts can be calculated thusly:
$$
\text{number of contracts} = \left( \frac{\beta_T - \beta_P}{\beta_f} \right) \cdot \left( \frac{V_p}{P_f} \right)
$$
$$
\text{number of contracts} = \left( \frac{\text{MD}_T - \text{MD}_P}{\text{MD}_f} \right) \cdot \left( \frac{V_p}{P_f} \right) \cdot (\text{yield beta})
$$

- The modifications achieved by these methods is rarely perfect, due to **basis risk**
  - This occurs when the item being hedged is not a good match for the hedging instrument
  - This causes the relationship between the portfolio and the derivatives purchased to change in unexpected ways:
    - The portfolio being hedged is different to the index on which the hedging instrument is based
    - The estimated beta and duration are incorrect
    - The results of the hedge are inspected at a time other than contract expiration (where future and spot prices are known)
    - The initial prices where not fair according to arbitrage formulae

- Synthetic positions make the use of derivatives to create positions equivalent to the purchasing of an actual asset, including resulting cashflows
  - A synthetic equity position combines equity futures with sufficient cash assets invested at the risk-free rate to "pay for" the position at expiration
  - A synthetic cash position combines selling equity futures with holding sufficient underlying securities to settle the position
  - Formulae for futures contract hedging can be used to construct these positions, with future values used in place of portfolio values
  - Futures can also be used to adjust from equity exposure to bond exposure by shorting stock index futures to eliminate systematic risk, and then purchasing bond futures
    - The inverse can be done to shift exposure from bonds to equities
  - Value can be effectively "transferred" from one asset class to another by converting exposure from one class, to cash, and then to the target class
  - **Pre-investing** involves taking long positions in futures contracts to create exposure to convert future cash flows into a synthetic position

- Exchange rate risk comes in three main forms
  - *Economic exposure* is a domestic exporter's loss of sales due to currency appreciation
  - *Translation exposure* is a domestic investor's loss of value in foreign assets due to foreign currency depreciation
  - *Transaction exposure* is loss due to exchange rate fluctuations reducing the value of foreign cash flows, or increasing the cost of foreign purchases