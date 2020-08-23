# Section 4 Homework - Using Pandas for Whale Analysis
        Repository for Unit 4 Homework
        
## Description of Project

In this project, we import and analyze a set of .csv files that contain returns for a number of stock portfolio. It is a combined analysis of "whale" portfolios, from investors with significantly large amounts of capital and algorithmic or "algo" portfolios, portfolios that use machine learning to try to outperform the market. These portfolios were compared against returns from the S&P 500, an index of stocks that represent the stock market. These portfolios are then weighted against a selection of new stocks, chosen by myself, to see if they outperform the portfolios.

## Findings

While all of the portfolios had unique attributes, the Algo 1 algorithmic portfolio did consistently beat the S&P 500 performance, with significantly lower volatility than some of the "whale" portfolios. It illustrates that, when the algortihm is written correctly, algo portfolios can offer substantial growth opportunity for clients that may be more sensitive to risk.

The Wilson Portfolio sought to examine the behavior of stocks in sectors that have shown growth during the Coranvirus pandemic. However, due to issues concatenating, I could not view the portfolio alongside with the whale/algo portfolios. I did however review the individual stocks performances against the portfolios. Long-Term I believe the Wilson Portfolio would not have outperformed the S&P and it would have been a very volatile portfolio long term, something which I as an investor am sensitive too. I did find it interesting that in reviewing the Sharpe Ratios, Square had an acceptable-good representation of risk-adjusted return when compared to the other stocks chosen for the Wilson Portfolio. Given that it is a fin-tech firm and was only founded in 2009, it demonstrates that fin-tech firms have a place in a risk tolerant portfolio, and should be considered for invesmtent as more of them head toward IPO.

## Aditional Learnings
Before I realized that the whale_analysis notebook was started in Jupyter, I started a sperate notebook, independent of it, and began commenting and planning my code for the project. I found that doing so had helped me visualize what I needed to do to get started. The whales_analysis notebook did have elements grouped differently, but I felt that in practice, it helped. I left the Whales notebook here for feedback on the "planning" stage of writing python code.

## Overcoming Struggles
I felt at first that I was moving at a relatively decent pace through the homework. I tried to continue on with the code even though I hit a few roadblocks along the way.

I realized finally that it's better to demonstrate that I understand the elements and get the code wrong, then try to have perfect code and not complete the assignment.

EX:1 I was struggling to understand how to pivot my dataframe to make a new pivottable. So I read the example from 4.1 over and over, until it made sense. I realized that my GoogleFinance data was already in the format that was being asked for. So I improvised, and downloaded the .csv files for AAPL and COST to make the table work.

EX2: I was able to read in individual .csv files for the stocks in my portfolio, but could not find a portfolio option in  GoogleFinance. I concatted the dataframes together, and found a weighted returns value, essentially creating my portfolio. I could not however concatenate it to the dataframe with the whale/algo portfolios. 

I attempted writing the dataframe to a .csv file (successful) and importing it back into the notebook, adding back an index, and re-naming columns. However, when I was able to concat the dataframe, but had a significant number of 'Nan' values both in my newly imported data, and the data that was provided for us to do the homework. I was unable to drop the number of 'Nans'. Instead of stopping, I moved forward with analysis of the individual stocks. For me, things not working correctly is difficult. But I realize I learn more from my mistakes than I do when I get things right. So, I look very forward to your feedback on this assignment.
