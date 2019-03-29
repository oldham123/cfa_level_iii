# Reading 17: Equity Market Valuation

## 17.A: Explain the terms of the Cobb-Douglass production function and demonstrate how the function can be used to model growth in real output under the assumption of constant returns to scale

- In *neoclassical* economics, the **Cobb-Douglas production function** is used in estimating total real economic output
  - In equity analysis, it can also be used to estimate future growth
$$
Y = A \cdot K^\alpha \cdot L^\beta
$$
    - $Y$ is real economic output
    - $A$ is total factor productivity
    - $K$ is capital stock
    - $L$ is labour input
    - $\alpha$ is the output elasticity of $K$
    - $\beta$ is the output elasticity of $L$
  - By applying several simple assumtions, the equation can be rearranged into the following:
$$
\frac{\Delta Y}{Y} \approx \frac{\Delta A}{A} + \alpha \cdot \frac{\Delta K}{K} + (1 - \alpha) \cdot \frac{\Delta L}{L}
$$
  - Research demonstrates that *constant returns to scale* is a reasonable assumption in this context

- **Total factor productivity (TFP)** is the ability of an economy to convert given inputs of labour and capital into real output
  - The **Solow residual** is the percentage change in **total factor productivity**, and is given by the following;
$$
\frac{\Delta \text{TFP}}{\text{TFP}} \approx \frac{\Delta Y}{Y} - \alpha \cdot \frac{\Delta K}{K} - (1 - \alpha) \cdot \frac{\Delta L}{L}
$$
  - Reasons for a change in TFP include:
    - A change to trade restrictions
    - A change to capital flows
    - A change to labour flows
    - A legal change
    - Natural resource discovery and extraction
    - Technological advancement

## 17.B: Evaluate the relative importance of growth in total factor productivity, in capital stock, and in labour input given relevant historical data

- When determining input values for the CD production function, it is important to ensure the historical periods used are appropriate given the period for which the inputs are being estimated
  - Changes in total factor productivity have the greatest impact on changes to economic growth
  - Changes to both labour and capital are mitigated somewhat by the output elasticities of each factor

## 17.C: Demonstrate the use of the Cobb-Douglas production function in obtaining a discounted dividend model estimate of the intrinsic value of an equity market

## 17.D: Critique the use of discounted dividend models and macroeconomic foecasts to estimate the instrinsic value of an equity market

- Dividend discount models require forecasts of an economy's growth rate as an input
  - In developed markets, the Gordon Growth dividend discount model is more appropriate 
    - Growth of dividends is closely related to the growth of the economy
    - This is because the amount of aggregate economic activity that the corporate sector is responsible for is unlikely to be volatile
    - Additionally, stable growth rates make the Gordon-growth dividend discount model more appropriate
    - Similarly, risk, and therefore the appropriate discount rate is also easier to determine
  - The H-model dividend discount model is best suited to developing markets, where analysts face issues such as:
    - Volatility of growth rates and risk
    - Volatile political and legal environments disrupting the relationship between dividend and economic growth rates
    - Less reliable economic data

- The Gordon Growth dividend discount model is given by:
$$
V_0 = \frac{D_1}{r - \bar{g}} = \frac{D_0 \cdot (1 + \bar{g})}{r - \bar{g}}
$$

- The H-Model for emerging economies is given by:
$$
V_0 = \frac{D_0}{r - g_L} \cdot \Big( (1 + g_L) + \frac{N}{2} \cdot (g_S - g_L) \Big)
$$
  - Each term denotes the following:  
    - $V_0$ is the intrinsic market value
    - $D_t$ is the dividend in period $t$
    - $r$ is the appropriate discount rate
    - $\bar{g}$ is the estimated long term growth rate
    - $g_L$ is the estimated *long* term sustainable growth rate
    - $g_S$ is the estimated initial *short* term higher growth rate
    - $N$ is the number of periods over which the growth rate is expected to linearly approach $g_L$ from $g_S$
  - Inputs are usually real values as opposed to nominal
    - The CD production function gives a real growth rate as the output
    - Real values are more easily comparable between economies

## 17.E: Contrast top-down and bottom-up approaches to forecasting the earnings per share of an equity market index

- Top-down forecasts make use of broader, *macroeconomic* data, and estimate future values of broader indicators such as benchmark indices
  - An analyst could inspect historical values of indices to determine if any are under or overvalued
  - An analyst could determine if the indices were moving with any momentum
  - The forecasted performance of the index can then be compared to general asset classes, sectors, or even individual securities

- Bottom-up forecasts begin with a focus on firm fundamentals
  - Individual companies are compared with the industry in which they reside
  - The mangement of the firm is assessed with regards to their capability and willingness to innovate
  - Following this, cash flow analysis can be used to determine a return estimate
  - The analysis can be performed for multiple firms, and then aggregated

- The appropriate approach depends on the asset selection strategy, and the inputs required for that process

- When comparing top-down and bottom-up approaches it is important to understand the differences between them, and the reasons why they may generate different estimates:
  - Econometric models used in top-down analysis may be improperly specified
  - Managerial expectations may impact the results of bottom-up analysis, since they are often inappropriately optimistic

## 17.F: Discuss the strengths and limitations of relative valuation models

## 17.G: Judge whether an equity market is under, fairly, or overevalued, using a relative equity valuation model

- The use of the relative values of assets involves **relative value models**
  - **The Fed model** assumes that the yield on long term Tresuries equals the operating earnings yield on the S&P 500
    - If the earnings yield is higher, this is interpreted as a sign that equity prices are too low, and vice-versa
    - Disadvantages include:
      - Ignorance of the equity risk premium
      - Assumption of zero earnings growth
      - Compares real and nominal values
    - To mitigate these disadvantages, rather than simply assuming the values should be equal, analysts observe the change of the ratio between them

- The **Yardeni model** is a variation of the **constant growth dividend discount model** that estimates the **equilibrium earnings yield**
  - Beginning with the following:
$$
P_0 = \frac{E_1}{r - g}
$$
  - We can rearrange to give:
$$
\frac{E_1}{P_0} = r - g
$$
  - The A-rated corporate bond yield is substituted as the required equity return, and the long-term growth rate of the S&P 500 (multiplied by a weighting factor determined using historical data) for the long-term growth rate gives final formulation of:
$$
\frac{E_1}{P_0} = Y_B - d \cdot \text{LTEG}
$$
  - If the market earnings yield is higher than the Yardeni earnings yield, then this implied that equities are underpriced
  - As compared to the Fed model, the Yardeni ratio substitutes the Treasury yield for the A-rated corporate bond yield minus some weighting of long term earnings growth
    - If the equity risk premium is historically high (high corporate bond yields compared to treasury yields) these ratios might provide different conclusions

- The **Cyclically Adjusted P/E Ratio (CAPE)** is the ratio of a broad market index against a trailing 10-year moving average of earnings
  - If above average, then this can be interpreted as a sign that equities are overvalued
  - When utilising the CAPE, it is important to adjust both inputs for inflation, by stating them in terms of the same base year
  - This model can capture the effects of business cycles, but fails to account for changes in accounting methods
  - Research also shows that abnormally high or low CAPE ratios can sustain for a long time, mitigating the value of the CAPE in developing short-term market expectations

- Two asset based models are referred to as **Tobin's Q** and **Equity Q**:
  - Tobin's Q is a ratio of market value of assets to replacement cost of assets
    - Intuitively this ratio should be 1, and a value greater than that implies that the firm's stock is overvalued
  - Equity Q is similar, but it replaces market value of assets with market value of equity
  - Both rations are expected to eventually revert to 1 as stock prices correct
    - This correction may not happen quickly