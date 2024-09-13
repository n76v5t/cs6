java c
ECMT 6002/6702: Econometric Applications
1 Practice problems
1. Consider the following linear regression model:
yt = α + βxt + ut.
A widely used goodness-of-fit measure is R2 = ESS/T SS, where

and ybt (resp. ut) is the fitted value (residual).
(i) Show that T SS = ESS + RSS.
(ii) Under what condition ESS = 0 (and hence R2 = 0)?
(iii) Consider the following two problems:

and

Note that (1.1) is obtained by restricting γ to zero in (1.2). If the optimal solution to (1.2) is given by (α*, β*, γ*) and γ* ≠ 0, (1.2) is smaller than (1.1). From this observation, we find that

Based on (1.3), find how R2reacts to inclusion of zt.
(iv) The results given in (iii) can be easily extended to the general case with k regressors. Based on this, discuss on limitation of R2 as a measure of goodnees-of-fit .
2. Consider the following simple linear regression model:
yt = α + βxt + ut
The OLS estimates of α and β are respectively given by
α = 1.2        β = −4.1                         (1.4)
The estimated standard error of β is
SE(β) = 0.8.                      (1.5)
(a) Suppose that we want to estimate the null hypothesis:
H0 : β = −4                          (1.6)
against
H1 : β ≠ −4.                             (1.7)
Compute the t-statistic to examine the above hypotheses and check if H0 is rejected at 5% significance level or not. Assume that T is sufficiently large and thus the OLS estimator is approximately normal.
(b) Compute the 95% confidence interval for β.
(c) Test H0 against H1 with 10% significance level.
(d) Test H0 against H1 : β < −4.1 with 5% significance level.
(Note) Quantiles of N(0, 1)

2 Empirical application
Consider the following model:

The relationship between yt and xt may be dependent on the university is private or public. To see this, the additional variable ztis added, i.e.,

where

Instructions:
1. Use the attached dataset. The dataset is considered in Wooldridge’s text book “Introductory Econometric代 写ECMT 6002/6702: Econometric Applications 2Prolog
代做程序编程语言s” and was collected from the FBI Uniform. Crime Report.
2. Compute the OLS estimates of α, β and γ. In R, lm(y ∼ X + 0) (or lm(y ∼ X)) can be used if y is the vector of yt and X is the (T × 3) data (independent variables) matrix discussed in class. You can easily do this in any statistical package but, I would recommend you compute those by constructing data matrix X and computing directly.
Note : The command lm(y ∼ X) automatically includes the vector of ones regardless of X contains it or not, while lm(y ∼ X + 0) does not add the vector of ones for estimation. Since X already contains the vector of ones by our construction, lm(y ∼ X + 0) may be more natural in R. But you can also use lm(y ∼ X) since R automatically ignores the first column vector of X in this case.
Depending on which software is used, the estimates can be slightly different. But they must be close to the following:
α = −36.07,        β = 21.16,      and          γ = −26.29.
3. Compute the standard errors of the OLS coefficients. In R, you can easily see all of these by summary(lm(y ∼ X + 0)). Depending on which software is used, the estimates can be slightly different. But they must be close to the following:
SE(α) = 59.723,    SE(β) = 2.189,     and    SE(γ) = 103.375.
You can also try direct computation, and this is actually easy. If X is the data matrix and s2is the variance of the OLS residuals, compute first
s2(X′X)−1              (2.2)
This will give you (3 × 3) matrix. The square-roots of the diagonal elements of this matrix are the standard errors. You can obtain s2 by mean((lm(y ∼ X + 0)$residuals)2). If your computations are correct, the results will be similar to

and thus approximately

4. This computing exercise is not mandatory; any computing code related to this application will not be asked in the exams. But you are strongly encouraged to work on this by yourself with your preferred statistical software (this will be helpful for your assignments).







         
加QQ：99515681  WX：codinghelp
