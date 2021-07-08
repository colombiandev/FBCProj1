# Project 1 – Investment Strategy Analysis
## Summary
For this project we wanted to look at how different investment strategies have performed relative to each other.  We decided that the best way to explore this was to find ETFs that were built around each of these strategies.  We trusted the finance professionals who built these ETFs to do a proper job to reflect the strategy that we were interested in looking at.  Just to be safe and make sure our analysis will be accurate we decided to find 3-4 ETFs that each follow the same strategy from different companies.  The holdings of each of these ETFs will be similar overall, but having multiple providers limits the chance of the data being skewed by an outlier in one of the ETFs.  

## Questions Asked
The questions that we wanted to ask of the data were the following:

§	How do each of the ETFs for each of the strategies correlate to each other?

§	How have the returns for each of the ETFs compared to each other?  

§	Which has the best return over the past 5 years? And the worst?

§	How risky is each strategy?

§	How does the risk compare to the returns?

§	How does the volume traded look compared to the returns that have been seen over the past 5 years?

## The Data
For the analysis, we downloaded .csv files of the 5-year historical data for each of the ETFs that corresponded to our strategies.  We used Morningstar’s ETF index to find the ETFs that we wanted to explore and then downloaded the data from the NASDAQ website where we felt we would be able to find the most complete and accurate data.  This made the cleanup process fairly straightforward once we imported the data to our workbooks.  Most of the tables that we created from the .csv files were complete and didn’t have many blank cells that we needed to drop, and then from there we merged the data frames of each individual ETF into one for each strategy containing the different ETFs from each company, and then merged the ETFs from each strategy into one data frame for each company that created them as well to give us something like this to work with:
 
(Above is a data frame with the daily closing price of the 20 year treasury bill ETFs as well as the data frame containing each ETF from Invesco, one from each strategy)

## The Analysis
After we imported and cleaned our data and created our data frames as explained above, we began the analysis.  For my own, I decided to begin with the correlation of the ETFs that I chose to represent each strategy.  This is where I noticed that for one of my ETFs for the 20-year treasury bill was actually an inverse of the actual one.  It was designed to act as if it was shorting the bonds rather than following and matching their returns.  I decided to keep it in there since I thought it was an interesting contrast to the rest of the analysis and just to see where it will take me.  Having 3 other ETFs that follow the same strategy allowed me to keep it and not skew the overall data of the analysis.  

After looking at the correlation I moved on to the percentage change in daily returns for each strategy and for each provider’s ETFs as well as the cumulative returns for everything and plotted what I found using hvplot to have an interactive chart.  

Next, I looked at the riskiness of the strategies.  For each I calculated the standard deviations, the volatility and the sharpe ratios to see how the risk of each strategy related to the returns that each have seen.  Then I plotted the sharpe ratios in a bar chart to have a visual representation. (The sharpe ratio describes how much excess return you receive for the extra volatility you endure for holding a riskier asset.  The riskier something is, the higher the return you want to see should the investment pay off)

After that I decided to look at the volume traded of each of the ETFs to see what the demand for each ETF looked like.  I started with the 5-year average to get a picture of which ones were traded more often and which ones were not, and then I looked at the average for each year that we pulled the data for, from 2016 to 2021. I also looked at the average closing price for these time frames to see if the higher volume had to do with demand for the product or if the price was significantly lower than the other options causing consumers to buy more shares for the same dollar value investment.  

## Our Conclusions 

For our conclusions we will bring it back to the questions that we wanted to ask of the data when we started the project which were the following: 

  
•	How have the returns for each of the ETFs compared to each other?  
•	Which has the best return over the past 5 years? And the worst?
•	How risky is each strategy?
•	How does the risk compare to the returns?


