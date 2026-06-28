# CAST 1.1.0

Latest run: 2026-06-28: https://github.com/r-devel/linux-arm64-checks/actions/runs/28309012007

```
Package: CAST
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Differences:
      `actual`: 27.69
    `expected`: 27.40
    
    ── Failure ('test-global_validation.R:20:3'): global_validation works with caret regression ──
    Expected `global_validation(model)` to equal `c(RMSE = 0.330787, Rsquared = 0.8400544, MAE = 0.2621827)`.
    Differences:
      `actual`: 0.341 0.830 0.271
    `expected`: 0.331 0.840 0.262
    
    
    [ FAIL 3 | WARN 0 | SKIP 20 | PASS 143 ]
    Error:
    ! Test failures.
    Execution halted

```
