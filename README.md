# Portfolio-Optimization

**Problem:** How does an optimally weighted portfolio compare to other asset allocation strategies?

I first look at the returns for stocks (daily, monthly, annually and cumulatively), then visualize daily returns using a simple histogram.

<img width="947" alt="returns image PO" src="https://user-images.githubusercontent.com/83718882/121433084-853b8c80-c949-11eb-8fa5-c6215a289fe9.png">

I then define the portfolio functions which will generate optimal weights, standard deviation and negative Sharpe Ratio function that we will minimize.

Creating an array of equally-spaced numbers that will represent our portfolio returns and annotate the five stocks on the plot allows us to visualize the Capital Allocation Line

<img width="961" alt="CAP PO" src="https://user-images.githubusercontent.com/83718882/121433101-8a98d700-c949-11eb-9d30-5af2bdf19cad.png">


<img width="930" alt="Portfolio PO" src="https://user-images.githubusercontent.com/83718882/121433109-8cfb3100-c949-11eb-8c1a-ecdf26d554c7.png">


Determines the optimal weights of five random stocks in a portfolio employing simple trading strategy. Runs a Fama French 4 factor simulation on two portfolios, equal weight and optimal weight to determine the most effective trading strategy.





```
  OLS Regression Results                            
==============================================================================
Dep. Variable:                 Opt-EW   R-squared:                       0.262
Model:                            OLS   Adj. R-squared:                  0.098
Method:                 Least Squares   F-statistic:                     1.597
Date:                Mon, 07 Jun 2021   Prob (F-statistic):              0.218
Time:                        16:51:51   Log-Likelihood:                 39.221
No. Observations:                  23   AIC:                            -68.44
Df Residuals:                      18   BIC:                            -62.76
Df Model:                           4                                         
Covariance Type:            nonrobust                                         
==============================================================================
                 coef    std err          t      P>|t|      [0.025      0.975]
------------------------------------------------------------------------------
Alpha          0.0113      0.012      0.936      0.361      -0.014       0.037
Beta          -0.3476      0.329     -1.057      0.304      -1.038       0.343
SMB           -0.7090      0.465     -1.523      0.145      -1.687       0.269
HML           -0.3529      0.603     -0.586      0.565      -1.619       0.913
UMD           -0.5959      0.489     -1.218      0.239      -1.624       0.432
==============================================================================
Omnibus:                        0.324   Durbin-Watson:                   1.987
Prob(Omnibus):                  0.850   Jarque-Bera (JB):                0.150
Skew:                           0.183   Prob(JB):                        0.928
Kurtosis:                       2.847   Cond. No.                         64.1
==============================================================================
```
