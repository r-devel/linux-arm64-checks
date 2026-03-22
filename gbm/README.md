# gbm 2.2.3

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411385745

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
    test_relative_influence.R.....    1 tests [0;32mOK[0m [0;34m4.9s[0m
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
