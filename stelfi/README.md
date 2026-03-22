# stelfi 1.0.2

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411816779

```
Package: stelfi
Check: tests

AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Differences:
      `actual`: -1.54
    `expected`: -1.32
    
    ── Failure ('test-fits.R:82:13'): LGCP model fitting (spatial) ─────────────────
    Expected `pars[3]` to equal 0.95.
    Differences:
      `actual`: 1.11
    `expected`: 0.95
    
    
    [ FAIL 2 | WARN 0 | SKIP 8 | PASS 14 ]
    Error:
    ! Test failures.
    Execution halted
```
