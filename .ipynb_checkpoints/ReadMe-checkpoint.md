# AI for Trading Nanodegree

This repository contains my projects and personal notes for the Udacity's AI for Trading Nanodegree course.

## Project 1 - Trading with Momentum Strategy
- Processing data
    - Loading and pivoting data
    - Resampling adjusted close prices to monthly frequency with Pandas resample() method
- Calculating log return of stocks' prices
    - Generating previous prices and 
    - Using Pandas shift() method to return previous or future returns in the time series (* close price of last day of the month is appropriate for the next day (month) trade)
- Generating trading signal
    - Getting top and bottom n performing stocks for each month
- Calculating projected returns of our trading signals
    - Computing net returns that the portfolio would return
- Peforming One-sided T-Test on the observed mean return 
    - T-statistic to check if we can reject the null hypothesis ($H_0$) that the actual mean return from the signal is zero
    - Computing the t-statistic, and then finding its corresponding p-value
    - Setting $\alpha = 0.05$, since it's a common value to use
    - Using Scipy.stats module to perform the t-test on the sample of portfolio returns
