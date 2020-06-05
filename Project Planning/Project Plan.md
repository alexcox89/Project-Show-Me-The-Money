	- Objective
		○ Provide custom data analysis based on input portfolio.  Analysis includes:
			§ YTD performance
			§ Performance over time (1Yr, 5Yr, etc)
			§ Cost basis
			§ Overall Gain/lose
			§ Comparison to S&P, input ticker
				□ Based on Sharpe Ratio
		○ Dashboard
			§ Pie Chart
				□ Current Industry
				□ Goal: Trends
			§ Performances compared to other portfolios
				□ Combined performance
				□ Beta
				□ P/E ratio
				□ Sharpe Ratio
				□ Profit Margin
				□ Cash
				□ Dividends
		○ Goal:
			§ Mean-variance optimization
            § Fama French regression analysis
		
	- API: Pull Stock
		○ Input:
			§ Ticker
			§ Date Range
		○ Output
			§ Daily Closing Price
			§ Current Beta
			§ Current P/E ratio
			§ Current Profit Margin
			§ Current Cash
			§ Dividends
			§ Industry type
      * Alpaca
      
	- Goal API/Function: mean-variance optimization

	- Input Portfolio:
		○ Ticker, Buy Date, Buy Price
		○ Ticker, Sell Date, Sell Price
		
	- Function: performance
		○ Input: 
			§ DataFrame
			§ Date Range - input from dashboard
		○ Output:
			§ Plot of performance for given date range
	
	- Function:  Industry Weights
		○ Input:
			§ Dataframe
			§ Goal: Specific Dates - input from dashboard
		○ Output
			§ Industry weight for portfolio
	
	- Function: Ticker Stats
		○ Input:
			§ Dataframe
			§ Goal: Specific Dates - input from dashboard
		○ Output
			§ Sliced dataframe with beta, P/E ratio, profit margin, cash, dividends
            
Resources:
- https://financialmodelingprep.com/developer/docs/
