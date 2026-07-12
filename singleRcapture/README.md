# singleRcapture 1.1.0

Latest run: 2026-07-12: https://github.com/r-devel/linux-arm64-checks/actions/runs/29176716781

```
Package: singleRcapture
Check: tests
AMD64: OK
    Running ‘tinytest.R’
ARM64: ERROR
    Running ‘tinytest.R’
  Running the tests in ‘tests/tinytest.R’ failed.
  Last 13 lines of output:
     call| expect_silent(dd <- estimatePopsize(formula = TOTAL_SUB ~ ., 
     call| -->    model = "zotnegbin", method = "optim", data = farmsubmission, 
     call| -->    controlMethod = controlMethod(maxiter = 5000, optimMethod = "Nelder-Mead", 
     call| -->        silent = TRUE)))
     diff| Execution was not silent. An error was thrown with message
     diff| 'missing value where TRUE/FALSE needed'
    ----- FAILED[xcpt]: test_singleRcapture.R<32--37>
     call| expect_silent(predict(dd, type = "mean"))
     diff| Execution was not silent. An error was thrown with message
     diff| 'object 'dd' not found'
    Error: 2 out of 428 tests failed
    In addition: Warning message:
    In family$devResids(y = observed, wt = priorWeights, eta = eta +  :
      Numerical deviance finder found worse saturated likelihood than fitted model. Expect NA's in deviance/deviance residuals.
    Execution halted

```
