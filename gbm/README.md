# gbm 2.2.3

Latest run: 2026-06-09: https://github.com/r-devel/linux-arm64-checks/actions/runs/27217229435

```
Package: gbm
Check: tests
AMD64: OK
    Running ‘tinytest.R’
ARM64: ERROR
    Running ‘tinytest.R’
  Running the tests in ‘tests/tinytest.R’ failed.
  Last 13 lines of output:
    
    test_relative_influence.R.....    0 tests    
    test_relative_influence.R.....    0 tests    
    test_relative_influence.R.....    0 tests    
    test_relative_influence.R.....    1 tests OK 5.0s
    ----- FAILED[data]: test_least_squares.R<68--69>
     call| expect_true(abs(mean(data2$Y - f.predict)) < 0.01, info = "LS: checking if Gaussian absolute error within tolerance.")
     diff| Expected TRUE, got FALSE
     info| LS: checking if Gaussian absolute error within tolerance.
    ----- FAILED[data]: test_least_squares.R<70--71>
     call| expect_true(sd(data2$Y - f.predict) < sigma, info = "LS: checking if Gaussian squared error within tolerance.")
     diff| Expected TRUE, got FALSE
     info| LS: checking if Gaussian squared error within tolerance.
    Error: 2 out of 5 tests failed
    Execution halted

```
