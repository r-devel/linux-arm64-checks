# pcreg 0.1.0

Latest run: 2026-05-31: https://github.com/r-devel/linux-arm64-checks/actions/runs/26701653647

```
Package: pcreg
Check: examples
AMD64: OK
ARM64: ERROR
  Running examples in ‘pcreg-Ex.R’ failed
  The error most likely occurred in:
  
  > ### Name: robust_pcreg
  > ### Title: Robust Principal Component Regression (Robust PCR)
  > ### Aliases: robust_pcreg
  > 
  > ### ** Examples
  > 
  > data(mtcars)
  > Result <- robust_pcreg(mtcars, y = "mpg")
  Warning in robustbase::covMcd(X) :
    The covariance matrix has become singular during
  the iterations of the MCD algorithm.
  There are 0 observations (in the entire dataset of 32 obs.) lying on
  the hyperplane with equation a_1*(x_i1 - m_1) + ... + a_p*(x_ip - m_p)
  = 0 with (m_1, ..., m_p) the mean of these observations and
  coefficients a_i from the vector a <- c(-0.3333333, 0, 0, 0, 0, 0,
  -0.6666667, -0.6666667, 0, 0)
  Error in eigen(mcd$cov, symmetric = TRUE) : 
    infinite or missing values in 'x'
  Calls: robust_pcreg -> eigen
  Execution halted

```
