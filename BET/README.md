# BET 0.6.0

Latest run: 2026-10-11: https://github.com/r-devel/linux-arm64-checks/actions/runs/38106877965

```
Package: BET
Check: tests
AMD64: OK
    Running ‘regression.R’
ARM64: ERROR
    Running ‘regression.R’
  Running the tests in ‘tests/regression.R’ failed.
  Last 13 lines of output:
    +     after <- .Random.seed
    +     ok(identical(fit,expected[[id]]$BEAST))
    +     set.seed(f$statistic_seed)
    +     repeat_fit <- BEAST(X,3,subsample.percent=f$fraction,B=f$B,lambda=f$lambda,
    +                         index=list(1L,2L),method="stat")
    +     ok(identical(fit,repeat_fit) && identical(.Random.seed,after))
    +     ok(identical(MaxBET(X,3,index=list(1L,2L)),expected[[id]]$MaxBET))
    +     ok(identical(MaxBETs(X,3,index=list(1L,2L)),expected[[id]]$MaxBETs))
    +     ok(identical(cell.counts(X,3),expected[[id]]$cell.counts))
    +     ok(identical(symm(X,3,print.sample.size=FALSE),expected[[id]]$symm))
    +     ok(identical(get.signs(X,3),expected[[id]]$get.signs))
    + }
    Error in ok(identical(fit, expected[[id]]$BEAST)) : isTRUE(x) is not TRUE
    Calls: ok -> stopifnot
    Execution halted

```
