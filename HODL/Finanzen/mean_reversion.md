---
title: Mean Reversion
date: 2025-06-03 10:46
tags: 
---

----

### Definition  
A time series that displays a tendency to drift toward its **long-term average** over time value

---

### Properties

- Stationary
- Change in the value of the time series in the next time period is proportional to the current value
- Such a time series is referred to as an **Ornstein-Uhlenbeck** process
- [ADF test](adf_test) rejects unit root

---

### **Ornstein-Uhlenbeck**
A *continuous* mean-reverting time series can be represented as followed:
$$
  dx_t=\theta(\mu-x_t)dt + \sigma dW_t
$$
$\theta:$ Rate of reversion to the mean\
$\mu:$ Mean value\
$\sigma:$ Variance of the process\
$W_t:$ Wiener Process or Brownian Motion

This equation states that the change of the price series in the next continuous time period
is proportional to the **difference between the mean and the current price**, with the addition 
of **Gaussian noise**






----

----
**Backlinks:**
- [📂Quants101](/📁Quants101)
