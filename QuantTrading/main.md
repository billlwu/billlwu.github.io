---
title: Quant Trading
---

I started reading *Trading and Exchanges* by Larry Harris, a finance professor at USC. [Here](/QuantTrading/TandE.md) are some notes. 

I started reading *Adaptive Martket Hypothesis* by Andrew Lo. [Here](/QuantTrading/AMH.md) are some notes. 

I'm going through the series of books by Earnest Chan: *Quantitative Trading*, *Algorithmic Trading*, *Machine Trading*. Below are my notes and all things trading related:

2020/Dec

Quantivity [blogpost](https://quantivity.wordpress.com/2011/02/21/why-log-returns/) on why log returns are nice. Definitions: 
- return = ![equation](https://latex.codecogs.com/svg.latex?%5Cinline%20r_i%20%3D%20%5Cfrac%7Bp_i-p_j%7D%7Bp_i%7D), where ![equation](https://latex.codecogs.com/svg.latex?%5Cinline%20j%5Cequiv%20i-1).
- log return = ![equation](https://latex.codecogs.com/gif.latex?%5Clog%281&plus;r_i%29%3D%5Clog%28%5Cfrac%7Bp_i%7D%7Bp_j%7D%29); this is daily log return.

Did an exercise using historic (i.e. realized) volatility of the S&P 500 to normalize its log return (which comes with negative skew!). Code and figures [here](SP_returns.html). An EWMA (with variable decay rate) was used to compute volatility. I followed procedures outlined in this [blogpost](https://mathbabe.org/2011/07/24/measuring-historical-volatility/).

Wonderful [post](https://mathbabe.org/2011/06/12/what-is-seasonal-adjustment/) about *seasonal adjustment* (i.e. for housing sales) and 2 different models for making predictions (one is causal via a rolling window approach and the other is not). 

"There are only a few basic kinds of [trading models](https://mathbabe.org/2011/07/02/asymmetrical-information/) encountered on Wall Street":
- chasing dumb money (revenge of the nerds)
- asymmetrical information (I know something you don't)
- market-making (HFT?)
- providing "insurance" (hedging)
- seasonality (any trend that repeats itself)
- taking advantage of macroeconomic misalignment (Soro's pound trade)
