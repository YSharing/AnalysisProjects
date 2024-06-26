# AnalysisProjects

This repository is for demostrating analysis projects.

1. "Portfolio_Monte_Carlo.ipynb". This project is utilizing monte carlo method to figure out the best weights with maximum Sharpe ratio and minimum Volatility for a portfolio with Magnificent Seven” (M7) stocks: Alphabet, Amazon, Apple, Meta, Microsoft, Nvidia and Tesla. (Pandas, Numpy, yFinance for stock price, matplotlib for displaying the randomized weights and frontier lines per return among randomized weights, fred for risk free rate from Federal Reserve Economic Data)

2. "Portfolio_Optimization.ipynb". This project is utilizing Scipy to figure out the optimized weights for each target returns from -10% to highest return of a signle stock portfolio in 200 intervals. Optimization are using these stock tickers ['SPY','BND','GLD','QQQ','IWM']. Finally show portfolio with maximum sharpe ratio and minimum volitility among optimizated weights. (Pandas, Numpy, yFinance for stock returns, Scipy for optimization, fred for risk free rate from Federal Reserve Economic Data, matplotlib for displaying the optimized weight and frontier line for each target returns)

3. "Portfolio_Optimization2.ipynb". Built on top of previous version, this project tries to answer a question: What is the best portfolio weights with non-cyclical stocks in (Communication Services, Consumer Staples, Energy, Health Care, Real Estate, Utilities) sectors amoung S&P 500, given additional constraints: pick from lowest 5 trailing P/E for each sector as undervalued stocks, and consider "debt to equity" ratio as risk since it will be expenisve for companies with high debt to equity ratio to finance their debt in higher and longer interest rate environment. Perform optimization like ESG rating (https://www.esgperspectives.com/Quant.html). Finally, show portfolio weight with lowest "risk". (Pandas, Numpy, BeautifulSoup for web scraping S&P 500 list with sector info, yFinance for stock price and PE ratio, Scipy for optimization, , fred for risk free rate from Federal Reserve Economic Data, matplotlib for displaying the portfolio weights) 

4. "SeasonalAnalysis.ipynb". This project tries to decompose "SPY" price history to observe if the movement of the board market has seasonality factor.  This project gets 5 years histroy from yFinace and resampling the data into weekly format. (Pandas, statsmodels for time series analysis, yFinance for stock returns)

5. "AssetPECompare.ipynb". This project tries to determine "cheap" stocks in technology sector by PEs.
  
For Fred API, you will need to get your own api key and save it in file "apikey" (without file extension) in order to use the function. The "apikey" file needs to be same folder as "CustomFinanceData.py". the First line of the "apikey" file is the api key from Fred account. You can create a free account by visiting "https://fred.stlouisfed.org/" and go to "My Account".   
