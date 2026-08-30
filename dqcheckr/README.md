# dqcheckr 0.3.0

Latest run: 2026-08-30: https://github.com/r-devel/linux-arm64-checks/actions/runs/33288778363

```
Package: dqcheckr
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Differences:
    `actual`:   TRUE 
    `expected`: FALSE
    
    ── Failure ('test-run-validation.R:83:3'): warning-severity findings message() and the run completes with a snapshot ──
    Expected `runs$render_status` to equal "success".
    Differences:
    `actual`:   "failed" 
    `expected`: "success"
    
    
    [ FAIL 2 | WARN 0 | SKIP 14 | PASS 1290 ]
    Error:
    ! Test failures.
    Execution halted

```
