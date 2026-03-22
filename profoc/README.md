# profoc 1.3.4

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411669709

```
Package: profoc
Check: tests

AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Differences:
    `actual`:   FALSE
    `expected`: TRUE 
    
    ── Failure ('test-predict.R:82:1'): (code run outside of `test_that()`) ────────
    Expected `all(preds[1:10, , ] == model_partial_1_preds)` to be TRUE.
    Differences:
    `actual`:   FALSE
    `expected`: TRUE 
    
    
    [ FAIL 2 | WARN 0 | SKIP 1 | PASS 161 ]
    Error:
    ! Test failures.
    Execution halted
```
