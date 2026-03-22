# DPQ 0.6-1

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411319306

```
Package: DPQ
Check: tests

AMD64: OK
    Running ‘bd0-tst.R’
    Running ‘chisq-nonc-ex.R’
    Running ‘dgamma-tst.R’
    Running ‘dnbinom-tst.R’
    Running ‘dnchisq-tst.R’
    Running ‘dt-ex.R’
    Running ‘expm1x-tst.R’
    Running ‘hyper-dist-ex.R’
    Running ‘log4p1p-exp.R’
    Running ‘pnbeta-tst.R’
    Running ‘pnt-prec.R’
    Running ‘pow-tst.R’
    Running ‘ppois-ex.R’
    Running ‘pqnorm_extreme.R’
    Running ‘qbeta-dist.R’
    Running ‘qbeta-tst.R’
    Running ‘qgamma-ex.R’
    Running ‘qPoisBinom-ex.R’
    Running ‘stirlerr-tst.R’
    Running ‘t-nonc-tst.R’
    Running ‘wienergerm_nchisq.R’
    Running ‘wienergerm-pchisq-tst.R’
ARM64: ERROR
    Running ‘bd0-tst.R’
    Running ‘chisq-nonc-ex.R’
    Running ‘dgamma-tst.R’
    Running ‘dnbinom-tst.R’
    Running ‘dnchisq-tst.R’
    Running ‘dt-ex.R’
    Running ‘expm1x-tst.R’
    Running ‘hyper-dist-ex.R’
    Running ‘log4p1p-exp.R’
    Running ‘pnbeta-tst.R’
    Running ‘pnt-prec.R’
    Running ‘pow-tst.R’
    Running ‘ppois-ex.R’
  Running the tests in ‘tests/ppois-ex.R’ failed.
  Last 13 lines of output:
    +       if(doExtras) {
    +         !okLD    || all.equal(pp,  pp. , tol = 1e-12)
    +         notXorLD || all.equal(pp,  ppSL, tol = 1e-12)
    +         notXorLD || all.equal(pp., ppSL, tol = 1e-14)# both ppoisD()  "fast" or "slow" should be very close
    +       } else {
    +         !okLD    || all.equal(pp,  pp. , tol = 1e-12)
    +       })
    + }
    Lam = 11400; M =   11850 :
    Error in plot.window(...) : need finite 'ylim' values
    Calls: plot -> plot.default -> localWindow -> plot.window
    In addition: Warning messages:
    1: In min(x) : no non-missing arguments to min; returning Inf
    2: In max(x) : no non-missing arguments to max; returning -Inf
    Execution halted
```
