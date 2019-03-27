# Reading 16: Capital Market Expectations

## 16.A: Discuss the role of, and a framework for, capital market expectations in the portfolio management process

- **Capital market expectations** come in two types:
  - **Macro expectations**
    - Generally involve expectations about performance of the economy as a whole
    - "Top-down"
  - **Micro expectations**
    - Generally involve expectations regarding individual asset selection
    - "Bottom-up"

- **Beta research** is the process of formulating capital market expectations due to its relation to *systemic risk*
  - It is relevant to the valuation ofassets such as equities and fixed-income instruments

- **Alpha research** is the process of attempting to generate excess returns by implementing asset-specific strategies

- There is a seven step process to formulating capital market expectations:
    1. Determine the set of expectations required due to investor chracteristics, including: 
       - Tax status
       - Asset classes allowed
       - Time horizon
    2. Determine drivers of performance for the relevant assets in order to devise a plausible range of future performance
    3. Construct or identify an appropriate valuation model, informed by the requirements of the model
       - Comparables approach
       - Fundamentals approach
    4. Collect the highest quality data available
    5. Assign values to each model input by analysing current investment conditions
    6. Formulate expectations
    7. Continuously evaluate results and refine the model

## 16.B: Discuss challenges in developing capital market forecasts

- Common problems in forecasting are:
  - Limitations of economic data
    - Time lag between collection and distribution can be as long as two years
    - Data is often revised even later on
    - Metholodologies and definitions change over time, making data noncomparable without adjustment
  - Error in measurements and bias
    - Transcription errors can be serious if they occur in one direction
    - The deletion of a series of returns due to poor performance can result in survivorship bias
    - Infrequent appraisal of illiquid assets can unnaturally smooth prices, biasing risk measures down
  - Limitations of historical estimates
    - Economic, political, demographical, and technological changes can reduce the predictive power of historical data
    - These *regime changes* can result in *nonstationary data*
    - Whilst a longer selected time period can be preferable, such a period is more likely to include regime changes
  - Use of ex post risk and return measures
    - Observing a stock price increase, without observing the perceived risks that kept prices lower before the price can lead to underestimating risk and overestimating returns
    - It is important to understand the nature of hindsight when evaluating data
  - Misidentification of trends
    - Patterns discovered in historic data are unlikely to recur, but can create biases
    - This is often a result of **data mining** where statistically significant relationships emerge by chance
    - Analysts should take time to identify an economic rationale for relationships they discover, and test conclusions with out-of-sample data
  - Not accounting for conditioning information
    - Analysts should be careful if their dataset has been collated over a variety of economic conditions, such as both recession and expansion
  - Misinterpretation of correlations as causal
  - Psychological traps
    - The **anchoring trap** causes information delivered first to be overweighted
    - The **status quo trap** causes the status quo to be overweighted
    - The **confirming evidence trap** overweights existing opinions
    - The **prudence trap** overweights conservative forecasts
    - The **recallability trap** overweights memorable events
  - Model and input uncertainty

## 16.C: Demonstrate the application of formal tools for setting capital market expectations, including statistical tools, discounted cash flow models, the risk premium approach, and financial equilibrium models

- Formal tools, applied to reputable data, will generate replicable forecasts
  - Examples of formal tools include:
    - Statistical tools
    - Discounted cash flow models
    - The risk premium approach
    - Financial equilibrium models

- **Statistical tools**
  - Descriptive statistics summarise
  - Inferential statistics predict
  - With **stationary data**, the past will be a reliable guide to the future
  - A return estimate for a single period uses the arithmetic average
  - A return estimate for multiple periods used the geometric average
  - Using a historical equity risk premium plus a bond yield is another approach
  - A **shrinkage estimate** weights another projection with a historical estimate
  - **Time series models** are used for volatility estimates, and assume past behaviour is a reasonable estimator of the future
  - **Multifactor models** use sensitivities and risk factors to forecast returns
    - Inputs can be divided into levels, with the first being composed of broad market factors, and further levels being more specific

- **Discounted cash flow models**
  - The principle behind these models is that any asset prices should equal the present value of cash flows
    - This emphasis on future cash flows is an advantage ofthe approach
    - They do not however account for specific economic conditions like supply or demand
  - The **Gordon Growth** model is a common application, used to deduce an expected return, given the current price, dividend, and growth rate:
$$\hat{R} = \frac{\text{Div}_1}{P_0} + g$$
  - The model can also be extended into the **Grinold and Kroner** model 
    - It accounts for inflation ($i$) changes in the percentage of stock outstanding ($S$) and changes in the $\frac{P}{E}$ ratio:
$$\hat{R} = \frac{\text{Div}_1}{P_0} + i + g -\Delta S + \Delta \left( \frac{P}{E} \right)$$
    - The model has three main components:
      - $\text{expected income return} = \left( \frac{D_1}{P_0} - \Delta S \right)$
      - $\text{expected nominal earnings growth} = i + g$
      - $\text{expected repricing return} = \Delta \left( \frac{P}E{} \right)$
  - The use of **YTM** as an expected return estimate for fixed income securities is supported by DCF analysis
    - YTM gives the return realised if ll cash flows are reinvested at the YTM and the bond is held to maturity

- **Build-up models**
  - These models begin with a risk free rate, and then add compensation for various risks, such as:
    - An **inflation premium**
    - A **default risk premium**
    - An **illiquidity premium**
    - A **maturity risk premium**
    - A **tax premium**

- **Financial equilibrium models**
  - These models assume that supply and demand are balanced, such that financial models will value securities accurately
  - An example would be the International Capital Asset Pricing Model, calculating the return on a given asset from the risk free rate, the expected return on the global market, and sensitivity of the stock to the global market:
    - $\hat{R} = R_F + \beta \cdot (\hat{R}_M - R_F)$
    - This model can be rearranged to give the risk premium by recalling two facts:
      - $\text{Cov(i,M)} = \rho_{i,M} \cdot \sigma_i \cdot \sigma_M $
      - $\beta_i = \text{Cov(i,M)}$
    - Therefore, $R_i - R_F = \rho_\text{i,M} \cdot \sigma_i \cdot \left( \frac{\hat{R}_M - R_F}{\sigma_M} \right)$
  - Singer and Terhaar then improve this model with adjustments for **illiquidity** and **segmentation**
    - Liquidity is usually not a concern in developed markets, except for particular asset types, such as real estate or private equity
      - A liquidity premium can be estimated by comparing the multi-period Sharpe ratio of the asset to that of the market as a whole, until a point in time at which the asset is liquid, where the difference is the premium
    - Most markets have some degree of segmentation, with developed markets being slightly less segmented
      - Reasons include *home country bias*, and restrictions on capital flows
      - Segmentation premiums can be calculated using a weighted average of a premium assuming full integration, and a premium assuming full segmentation
        - Note that full segmentation yields a premium simply equal to $\sigma_i \cdot \left( \frac{\text{ERP}_M}{\sigma_M} \right)$, since the relevant global market is simply the market of the asset, with a correlation of 1

## 16.D: Explain the use of suvery and panel methods and judgement in setting capital market expectations

- Surveys can be undertaken of economists and analysts, to aggregate their expecations together
  - If the group included remains consistent, then this is referred to as a **panel method**

## 16.E: Discuss the inventory and business cycles and the effects that consumer and business spending and monetary and fiscal policy hve on the business cycle

- **Inflection points** are points in time where risk, and potential returns, may increase, due to broader economic changes
  - They can be identified by understanding the business cycle
  - Growth has two main components:
    - **Cyclical** short term effects
      - Cyclical growth is driven by the **inventory cycle** and the **business cycle**
      - The inventory cycle lasts between two and four years, and the business cycle lasts between nine to eleven years, although significant events can disrupt them
    - **Trend-growth** long term effects

- Cyclical growth is driven by measures of broad economic activity, including:
  - **GDP**, measured in real teams
  - The **output gap** (i.e. the difference between potential and current real GDP)
  - **Recessions**, and their frequency and persistence

- The inventory cycle is usually measured with the inventory to sales ratio
  - Increased confidence leads to anticipation of sales and increased inventories relative to sales
    - This has positive knock-on effect on employment, and growth
  - Eventually some factor will cause sales to fail to meet expectations, and inventories decline
    - When inventory peaks, growth slows as business try to sell off their inventory
    - When invetory hits a trough, growth spikes as businesses add to their stock

## 16.F: Discuss the effects that the phases of the business cycle have on short-term and long-term capital market returns

- By selecting assets that generate higher returns during troughs in the business cycle investors can supplement their incomes in tough economic conditions
  - Examples would be fixed income assets, and defensive stocks, or other assets with low risk premiums

- The business cycle has five main stages:
  - Initial recovery
    - Lasts several months
    - Features rising business confidence
    - Low interest rates and/or budget deficits provide government stimulus
    - The output gap is larger than usual
    - Short-term interest rates are low, or falling
    - Bond yields are hitting a trough
    - Stock prices are rising
    - Riskier assets perform well
    - Inflation falls
  - Early expansion
    - Can last up to several yers
    - Growth increases whilst inflation remains low
    - Confidence and inventories are both rising
    - Output gap begins to narrow
    - Bond yields are flat or rising
    - Stock prices rise
  - Late expansion
    - High confidence, employment, and growth
    - Little to no output gap
    - Increasing inflation, short-term interest rates, and bond yields
    - Contractionary monetary policy
    - Stock prices begin to peak, with increasing volatility
  - Slowdown
    - Can last up to a year
    - Confidence, stock prices, and inventory levels decline
    - Inflation continues to rise
    - Short-term interest rates and bond yields peak
    - Yield-curve may invert
  - Recession
    - Can last from 6 months to a year
    - Large declines in inventory, confidence, nd prodits
    - Unemployment and bankruptcy increase
    - Inflation peaks
    - Short-term interest rates and bond yields start to fall
    - Stock prices may eventually begin to rise in anticipation of the end of the recession

- **Inflation** is the increase in the market pricing level, and typically accelerates near the peak of the business cycle
  - **Disinflation** is a deceleration in the rate of inflation, which usually occurs at the onset of recession
  - **Deflation** is a reduction in the pricing level, and is a severe economic problem
    - Default is encouraged
    - Panic-selling can be triggered
    - Reduced scope to increase the money supply due to near-zero interest rates

- Consumer spending dominates over business spending in terms of contribution to GDP
  - Consumer spending is heavily seasonal, and primarily driven by after-tax income
  - Undertanding savings behaviour is also critical to predicting consumer spending, since spending is given by income less savings
    - Saving is negatively correlated with consumer confidence

- Business spending is more volatile, but a peak in inventory spending is a relatively bearish indicator, signalling that businesses may have overspent relative to sales

## 16.H: Demonstrate the use of the Taylor rule to predict central bank behaviour

- The primary goal of monetary policy is to ensure that growth remains as close to the long-run sustainable rate as possible
  - Higher growth rates cause inflation to rise, and so restrictive monetary policy tends to be used towards the end of expansions
  - Encouraging additional growth can be done by reducing interest rates
    - This increases both business and consumer spending, as well as bond and stock prices
    - Additionally, currency value can depreciate, increasing exports
  - The **equilibrium interest rate** is the rate at which inflation and growth are balanced, and is alo referred to as the **neutral rate**
    - One way of estimating it is to add the growth rate and targeted inflation rate together

- **The Taylor Rule** embodies these principles, and can be used to predict central bank behaviour, where $r$ denotes interest rates, $i$ denotes inflation, and $\text{GDP}$ denotes growth:

$$
r_\text{target} = r_\text{neutral} + \frac{1}{2} \cdot (\text{GDP}_\text{expected} - \text{GDP}_\text{trend}) + \frac{1}{2} \cdot (i_\text{expected} - i_\text{trend})
$$

- **Negative interest rates** amount to payments in return for being abl to maintain deposits at some financial institution
  - For a time, zero was regarded as the lowest sustainable interest rate, since depositors would simply convert to holding cash instead
  - As depositors swap to cash, institutions are focrced to offer higher interest rates
  - In reality, there was a failure to account for an effective **convenience premium** on being able to make deposits, such that a large transfer to cash didn't occur, even as rates fell to negative values

- **Quantitative easing** involved central banks making large injections of funds into the commercial banking system, in the hope that they would stimulate economic activity by increasing lending
  - Combined with negative interest rates, it ould be more attractive to spend or invest the funds
  - In order for this experimental combination of policies to work, market participants must believe that purchases made now will provide a positive net economic benefit in the future
  - However, negative interest rates can complicate the process of forming capital market expectations
    - If the risk free rate is negative, a policy neutral rate derived using the Taylor Rule becomes more appropriate
    - Multiple path projections for how the negative rates will eventually transistion to a long term stable rate should be considered
    - Sourcing comparable historical data in order to analyse such a period can be difficult since negative interest rates represent such an irregular economic regime

- Governments can also utilise **fiscal policy** to stimulate economies, by decreasing taxes, and/or increasing spending
  - It is important to note that maintaining a deficit of a certain size does not stimulate the economy, but *increasing* the deficit does
  - Additionally, expansion of the economy will have a natural contractionary effect on the deficit that is not restrictive
    - Only deficit changes driven directly by government policy can act as stimulus

## 16.I: Interpret the shape of the yielf curve as an economic predictor and discuss the relationship between the yield curve and fiscal and monetary policy

- The relationship between interest rates and debt maturities is captured by the **yield curve**
  - Both the central bank, and the economy itself, can have impacts on the yield curve
  - With expansive fiscal and monetary policy, the yield curve slopes upwards
  - When both are restrictive, the yield curve slopes downward
  - If fiscal and monetary policy conflict, the impact on the economy is less clear
    - If monetary policy is restrictive then the curve will tend towards flatness
    - If it is expansive however, the curve may tend towards moderate steepness

## 16.J: Identify and interpret the compoentns of economic growth trends and demonstrate the application of economic growth trend analysis to the formulation of capital market expectations

- The **long-term trend growth rate** functions as an effective limit on growth, and is determined by:
  - **Population**
    - Population growth, or demographic shifts that increase the amount of labour available allow for faster growth
  - **Economic factors**
    - Increased productivity, or greater efficiency in capital allocation can also provide for faster growth

- Develop economies usually grow at a stable rate, whilst emerging economies grow more erratically
  - The most important factor is stability in consumer spending
    - According to the **wealth effect**, spending increases as wealth increases
    - In contrast, the **permanent income hypothesis** says that long-term expectations are the biggest factor in driving consumer spending

- Government policies that can drive long-term growth include:
  - Avoiding large, persistent government deficients
    - This does not preclude counter-cyclical fiscal policy, but the *twin deficit problem* should be avoided
    - A large deficit funded through foreign borrowing can leads to imports that exceed exports, causing the economy to overheat
  - Minimised intervention in capital markets
  - Preservation of competitive markets
  - Investment in infrastructure
  - Simplified, clear tax codes

## 16.K: Explain how exogenous shocks may affect economic growth trends

- Whilst government policy is a significant factor in the state of the economy, short-term external factors are also important
  - Conflict, supply shocks and weather events, and financial crashes are all examples of these
  - **Exogenous shocks** originate from outside an economy's normal state, and are usually unanticipated and not priced into markets
  - It is not impossible for shocks to benefit economies, they are usually not positive events, and they also often spread from one market to another (**contagion**)

## 16.L: Identify and interpret macroeconomic, interest rate, and exchange rate linkages between economies

- Globalisation is deepening the economic links between countries
  - The resulting change is more stark for smaller, or less diversified economies
  - Examples of **macroeconomic links** include:
    - International capital flows
      - As an economy slips into recession, investment to international partners may fall
    - International trade
      - If a trading partner's imports fall, a trading partner may no longer be able to afford their current level of imports
    - Interest and FX rates
      - FX pegs can produce strong links, as maintaining an exchange rate forces one country to adopt the economic policies of another
      - FX pegs cause interest rates of the pegging country to exceed the pegged country, with the size of the discrepancy reflecting investor confidence in the integrity of the peg
        - If confidence falls, the currency becomes less attractive and the value falls
        - To maintain the peg interest rates must rise, as compensation for continuing to hold the currency

## 16.M: Discuss the risks faced by investors in emerging-market securities and the country risk analysis techniques used to evaluate emerging market economies

- Emerging markets generally involve taking on higher amounts of risk, and hence generating higher returns
  - This investment must often take the form of actual physical infrastructure, or human capital
  - This investment is usually financed through borrowing in foreign markets
  - Additionally emerging economies generally have unstable politics, with the lack of a substantial middle class with the capability to agitate for reform
  - Emerging economies are often heavily dependent on the sale of specific commodities, and are undiversified, leaving them subject to shocks

- Before investing in emerging markets, the following should be considered:
  - Is the government enacting sound monetary and fiscal policies?
    - Deficit to GDP ratios greater than 4% are a sign of significant credit risk
  - What level of growth is expected?
    - Growth rates above 4% should be required as compensation for greater than average risk
    - Growth rates below this can be a troubling indicator
    - Taxation, trade restrictions, and capital flow restrictions are all important considerations
  - Are currency values stable?
    - Volatile currency values can jeopardise confidence
    - OVervaluation can provide means to artificially stimulate the economy through excessive borrowing
  - Is the amount of leverage appropriate?
    - Debt is a necessary component of growth in emerging markets, but it should still be kept within acceptable levels
    - Debt to GDP ratios exceeding 50% are troubling, as are debt to current account receipts exceeding 200%
  - Are reserves of foreign currency sufficient to service short term debt?
    - Debt from foreign nations must often be paid in foreign currencies
    - If the value of reserves fall below the debt due within 12 months, this is a sign that default may be likely
  - Are structural reforms likely?
    - If prospects for an improvement in the legal environment that firms operate within are strong, then investor confidence will rise

## 16.N: Compare the major approaches to economic forecasting

- **Econometric analysis**
  - Often features many variables
  - Easily reused following model specification
  - Produced a quantifiable output
  - Complex, and difficult to specify
  - Dependent on accurate choices of inputs
  - Struggles to predict recessions
  - Expert interpretation of the output may be required

- **Economic indicators**
  - Easy to understand
  - Readily available data
  - Can be chosen according to specific forecasting objectives
  - Supported by research
  - Results can be inconsistent

- **Checklist approach**
  - Less complex than the use of econometrics
  - Allows for a mix of econometric analysis with human judgement
  - Introduces subjectivity into the analysis

## 16.O: Demonstrate the use of economic information in forecasting asset class returns

## 16.P: Explain how economic and competitive factors can affect investment markets, sectors, and specific securities

- Following the formation of overall capital market expectations, the next step is to derive expectations regarding the retrusn of various asset classes

- **Cash intruments** refer to short-term debt (maturities below a year)
  - Longer maturities, as well as lower creditworthiness, both increase risk, and provide higher returns
  - Strong expectations regarding interest rates, as well as overall economic health, may lead an investor to switch to the higher risk instruments

- **Credit risk-free bonds** are sovereign fixed income assets
  - Yields include a real yield, and also factor in inflation expectations
  - An increase in growth expectations increases yields due to an anticipated greater demand for debt to finance demand and investment

- **Credit risky bonds** are comporate fixed income assets
  - Stripping out the yield of sovereign assets with similar maturities can help determine the spread

- **Emerging market government bonds** are similar to credit risk-free bonds
  - However, they are usually riskier, and they are often denominated in a non-domestic currency

- **Inflation indexed bonds**
  - Several sovereign fixed income assets are indexed from inflation to shift inflation risk from the buyer of the bond back onto the issuer
  - Yields generally track economy growth, and are affected by supply and demand, since the market for them is fairly small
  - Additionally, yields fall with increasing inflation, as the desire to be isolated from inflation risk increases, and lower yields are required to compensate investors

- **Common stock**
  - Since the value of a stock ought to be predicated on the present value of future cash flows, this can be used as a guide to forming expectations about returns on a given stock
  - The business cycle primarily determines short term growth, although this may depend on whether an exact stock is non-cyclical, or defensive
  - Early in expansion, sales are increasing whilst input costs are more static, leading to stock price increases
  - Later in the expansion, input costs may also start to rise, causing earnings growth to slow

- **Emerging market stocks**
  - Both risk and return are higher with stocks in emerging markets
  - They are however reasonably closely linked to business cycles in developed markets due to contagion

## 16.Q: Discuss the relative advantages and limitations of the major approaches to forecasting exchange rates

- Currency values are a result of supply and demand forces, in turn a result of trade and capital flows between countries
  - Suppose country A imports more from country B than they sell to country B
    - Effectively this will amount to consumers in country A selling currency A for currency B, in order to buy from country B
    - This is the aggregate impact of stores in country A paying currency B for the imported goods to sell
  - Alternatively, suppose bonds from country A have an attractive risk and return profile
    - Investors will sell their domestic currency, so that they can use currency A to buy the bonds

- Capital flows can be volatile (although less so if invested in physical assets), as can currency values, making them difficult to forecast
  - **Relative purchasing power parity** states that if there are inflation differences between economies, there will be currency value differences
    - It only holds in the long term, and even then only approximately, since its effects can be obscured by other influences
  - **Relative economy strength** states that a favourable investment climate increases demand for a country's currency, increasing its value
    - High short-term interest rates can have the same impact, even if there is broad agreement that this has caused the currency to be overvalued
  - The **capital flows approach** advocates focusing primarily on long-term capital flows, as opposed to more short-term factors in other approaches
    - Note that this approach would support a different conclusion to the relative strength approach when considering short-term interest rates
  - The **savings-investment balance approach** is an attempt at explaining long term currency divergences from theoretical estimates
    - Investments must be funded with savings, and if investment exceeds savings, additional inflows are required
    - Persistently high currency values are necessary to attract and keep this capital inflow
    - Eventually, once the economy slows, investment reduces and savings increase, at which point the currency devalues