---
title: Quant Trading
---

I'm going through the series of books by Earnest Chan: *Quantitative Trading*, *Algorithmic Trading*, *Machine Trading*. Below are my notes and all things trading related:

2020/Dec

Quantivity [blogpost](https://quantivity.wordpress.com/2011/02/21/why-log-returns/) on why log returns are nice. Definitions: 
- return = ![equation](https://latex.codecogs.com/svg.latex?%5Cinline%20r_i%20%3D%20%5Cfrac%7Bp_i-p_j%7D%7Bp_i%7D), where ![equation](https://latex.codecogs.com/svg.latex?%5Cinline%20j%5Cequiv%20i-1).
- log return = ![equation](https://latex.codecogs.com/gif.latex?%5Clog%281&plus;r_i%29%3D%5Clog%28%5Cfrac%7Bp_i%7D%7Bp_j%7D%29); this is daily log return.

Did an exercise using historic (i.e. realized) volatility of the S&P 500 to normalize its log return (which comes with negative skew!). Code and figures [here](SP_returns.html). An EWMA (with variable decay rate) was used to compute volatility. I followed procedures outlined in this [blogpost](https://mathbabe.org/2011/07/24/measuring-historical-volatility/).

Wonderful [post](https://mathbabe.org/2011/06/12/what-is-seasonal-adjustment/) about *seasonal adjustment* (i.e. for housing sales) and 2 different models for making predictions (one is causal via a rolling window approach and the other is not). 
