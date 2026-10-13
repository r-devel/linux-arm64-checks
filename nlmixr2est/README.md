# nlmixr2est 7.2.0

Latest run: 2026-10-13: https://github.com/r-devel/linux-arm64-checks/actions/runs/38464325448

```
Package: nlmixr2est
Check: examples
AMD64: OK
ARM64: ERROR
  Running examples in ‘nlmixr2est-Ex.R’ failed
  The error most likely occurred in:
  
  > ### Name: nlmixr2Eval_
  > ### Title: Create a gradient function based on gill numerical differences
  > ### Aliases: nlmixr2Eval_ nlmixr2Unscaled_ nlmixr2Grad_ nlmixr2ParHist_
  > ###   nlmixr2GradFun
  > ### Keywords: internal
  > 
  > ### ** Examples
  > 
  > 
  > func0 <- function(x){ sum(sin(x))  }
  > 
  > ## This will printout every iteration or when print=X
  > gf <- nlmixr2GradFun(func0)
  > 
  > ## x
  > x <- (0:10)*2*pi/10;
  > gf$eval(x)
  |-----+---------------+-----------+-----------+-----------+-----------|
  |    #| Objective Fun |        t1 |        t2 |        t3 |        t4 |
  |.....................|        t5 |        t6 |        t7 |        t8 |
  |.....................|        t9 |       t10 |       t11 |...........|
  |    1|-1.2246468e-16 |     0.000 |    0.6283 |     1.257 |     1.885 |
  |.....................|     2.513 |     3.142 |     3.770 |     4.398 |
  |.....................|     5.027 |     5.655 |     6.283 |...........|
  [1] -1.224647e-16
  > gf$grad(x)
  Error: On initial gradient evaluation, one or more parameters have a zero gradient
  Change model, try different initial estimates or try derivative free optimization)
  Execution halted

```
