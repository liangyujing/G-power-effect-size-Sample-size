# 1. 用G power: Syntax

## [1] -- Thursday, November 08, 2018 -- 19:06:44
   F tests - ANCOVA: Fixed effects, main effects and interactions

### Analysis: A priori: Compute required sample size

### Input: 
Effect size f = 0.3692745
α err prob = 0.05   ## α
Power (1-β err prob) = 0.90   ## Power
Numerator df = 1
Number of groups = 4
Number of covariates =

### Output: 
Noncentrality parameter λ = 10.9090925   ## λ
Critical F = 3.9667598    ## F
Denominator df = 76
Total sample size = 80
Actual power = 0.9033556


# 2. 用R
## 知道power 算被试数
##How many respondents per country are needed to obtain a power of  and ?
##答案：93 (per group)
##R code: 
pwr.anova.test(k=2,f=.24,power=.90,sig.level = .05)

## 知道被试数算power 
##If 40 participants per country are included, is the power acceptable?
##答案：No. The power is only .56.
##R code: 
pwr.anova.test(k=2,f=.24,n=40,sig.level = .05)
