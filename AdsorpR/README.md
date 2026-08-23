# AdsorpR 0.1.0

Latest run: 2026-08-23: https://github.com/r-devel/linux-arm64-checks/actions/runs/32608877698

```
Package: AdsorpR
Check: examples
AMD64: OK
ARM64: ERROR
  Running examples in ‘AdsorpR-Ex.R’ failed
  The error most likely occurred in:
  
  > ### Name: nonlinear_bet
  > ### Title: Non-linear BET Model
  > ### Aliases: nonlinear_bet
  > 
  > ### ** Examples
  > 
  > Ce <- c(1, 2.5, 4, 5.5, 7)
  > Qe <- c(0.4, 1.0, 1.7, 2.3, 2.7)
  > result <- nonlinear_bet(Ce, Qe)
  Warning in nls(Qe ~ (Qm * Cb * Ce)/((Cs - Ce) * (1 + (Cb - 1) * Ce/Cs)),  :
    singular gradient
  Error in chol2inv(object$m$Rmat()) : 
    element (2, 2) is zero, so the inverse cannot be computed
  Calls: nonlinear_bet -> summary -> summary.nls -> chol2inv
  Execution halted

```
