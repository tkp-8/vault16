---
title: Statistical_Learning
date: 2025-06-03 05:30
tags: 
---

----

### Definition 

*Statistical learning* ist the ability to extract regularities from the environment and learn 
from data

In a quantitative sense, we attempt to model the behaviour of an **outcome** or **response** based 
on a set of **predictors** or **features** assuming a relationship between the two

Let $Y$ be a response with $p$ different features $x_{1},x_{2},\ldots ,x_p$. Let $X$ be a $p$-dimensional
vetor, representing the features. $X=(x_{1},x_{2},\ldots ,x_p)$. The model of our relationship is
given by 
$$
  Y=f(X)+\epsilon
$$
Where $f$ is an unknown function of the predictors and $\epsilon$ represents an **error** or **noise** term


---

### Goal of Statistical Learning
**Estimating** the form of $f$ nased on the observed data and to **evaluate** how accurate those estimates are

---

### Prediction and Inference
*Prediction* is concerned with predicting an estimate response $\hat{Y}$ based on a newly observed 
predictor $X$. As long as the estimate responses are close to the true responses, the functional form of
$f$ is unimportant. Instead, we use the estimate $\hat{f}$ of $f$, of which the error is ideally reduced up to an irreducible extent 
$$
  \hat{Y}=\hat{f}(X)
$$
*Inference* is concerned with the situation where there is a need to understand the relationship 
between $X$ and $Y$ and hence its **exact form** must be **determined**.

---

### Parametric and Non-Parametric Models
In order to generate $\hat{f}$, we often consider a data set of the form
$$
  \{(X_{1},Y_{1}),(X_{2},Y_{2}),\ldots ,(X_N,Y_N)\}  
$$
A data set of this form is known as **training data** since it will be used to train a particular
statistical model that belongs to either of the following broad categories:

##### Parametric Models
- Require the **specification** or **assumption** of the form of $f$
- linear / non-linear

**Linear Model**\
Reduces the problem to that of estimating a coefficient vector $\beta=(\beta_{0},\beta_{1},\ldots ,\beta_p)$ of length $p+1$, where 
$\beta_{0}$ is the intercept hence $p+1$
$$
  Y\approx \hat{\beta}^{T}X=\beta_{0}+\beta_{1}x_{1}+\cdots+\beta_px_p \\
(^T\texttt{for Transpose)} 
$$

- Can lead to poor estimates, due to its **unflexible** nature
- Chosing alternate forms for $\hat{f}$ increases flexibility, but can cause a situation known as **overfitting**

##### Non-Parametric Models

- Potential of fitting a wider range of possible forms for $f$
- Need of an extensive amount of data points

---

### Supervised and Unsupervised Learning

##### Supervised Model
- Requires for each $X_j$ an associated $Y_j$  
- Supervision occurs when the model for $f$ is *trained* or *fit* to this data
- e.g OLS algorithm to train a linear regression model

##### Unsupervised Model
- No corresponding response $Y_j$ for any predictor $X_j$
- More Challenging but extremely powerful

---

### Techniques

- [Regression](regression)
- [Classification](classification)
- [Time_Series_Models](time_series_models)








----

----
**Backlinks:**
- [📂Quants101](/📁Quants101)
