---
title: Quant Trading
---

I'm going through the series of books by Earnest Chan: *Quantitative Trading*, *Algorithmic Trading*, *Machine Trading*. Below are my notes and all things trading related:

2020/Dec

Quantivity [blogpost](https://quantivity.wordpress.com/2011/02/21/why-log-returns/) on why log returns are nice. Definitions: 
- return = ![equation](https://latex.codecogs.com/svg.latex?%5Cinline%20r_i%20%3D%20%5Cfrac%7Bp_i-p_j%7D%7Bp_i%7D), where ![equation](https://latex.codecogs.com/svg.latex?%5Cinline%20j%5Cequiv%20i-1).
- log return = ![equation](https://latex.codecogs.com/gif.latex?%5Clog%281&plus;r_i%29%3D%5Clog%28%5Cfrac%7Bp_i%7D%7Bp_j%7D%29); this is daily log return.

[Historic volatility](https://mathbabe.org/2011/07/24/measuring-historical-volatility/): need some concept of return (log returns will do), weighting scheme (exponential, to simulate how people forget), running sum to save memory. If we compute the S&P 500 log returns from 2008.1 to 2011.1, there's crazy volatility caused by the financial crisis. This can be normalized with EWMA to behave better.

Important to distinguish between *alpha model* and *risk model*. Alpha model describes how you make money; risk model describes the downside risk exposure. 
