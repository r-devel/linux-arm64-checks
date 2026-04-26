# mig 2.0

Latest run: 2026-04-26: https://github.com/r-devel/linux-arm64-checks/actions/runs/24946064241

```
Package: mig
Check: tests
AMD64: OK
    Running ‘tinytest.R’
ARM64: ERROR
    Running ‘tinytest.R’
  Running the tests in ‘tests/tinytest.R’ failed.
  Last 13 lines of output:
    test-loocv.R..................    2 tests OK 
    test-loocv.R..................    2 tests OK 
    test-loocv.R..................    2 tests OK 
    test-loocv.R..................    2 tests OK 
    test-loocv.R..................    2 tests OK 
    test-loocv.R..................    3 tests OK 9ms
    ----- FAILED[data]: test-derivatives.R<22--25>
     call| expect_equal(max(abs(mig_loglik_grad(x = samp, xi = xi, Omega = Omega, 
     call| -->    beta = beta) - t(apply(samp, 1, function(x) {
     call| -->    numDeriv::grad(func = dmig, x = x, xi = xi, Omega = Omega, 
     call| -->        beta = beta, log = TRUE)
     call| -->})))), 0)
     diff| Expected '0', got '9.75088642052313e-08'
    Error: 1 out of 21 tests failed
    Execution halted

```
