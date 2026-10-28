# INLAcircular 1.0.0

Latest run: 2026-10-28: https://github.com/r-devel/linux-arm64-checks/actions/runs/40726818776

```
Package: INLAcircular
Check: tests
AMD64: OK
    Running ‘test-bessel-i.R’
    Running ‘test-direct-inla-lavm.R’
    Running ‘test-distribution-missing.R’
    Running ‘test-inla-availability.R’
    Running ‘test-inlacc-copy-prior.R’
    Running ‘test-lavm-control.R’
    Running ‘test-lkj-api.R’
    Running ‘test-pc-card-wc.R’
    Running ‘test-pc-vm.R’
ARM64: ERROR
    Running ‘test-bessel-i.R’
  Running the tests in ‘tests/test-bessel-i.R’ failed.
  Last 13 lines of output:
    > precision_result <- withCallingHandlers(
    +   bessel_i(rep(6627434193491816, 2), 1e16),
    +   warning = function(w) {
    +     precision_warnings <<- c(precision_warnings, conditionMessage(w))
    +     invokeRestart("muffleWarning")
    +   }
    + )
    > stopifnot(
    +   length(precision_warnings) == 1L,
    +   grepl("accuracy", precision_warnings, fixed = TRUE),
    +   all(is.finite(precision_result)),
    +   all(precision_result > 0)
    + )
    Error: length(precision_warnings) == 1L is not TRUE
    Execution halted

```
