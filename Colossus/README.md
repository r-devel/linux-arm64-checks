# Colossus 1.4.10

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411284418

```
Package: Colossus
Check: tests

AMD64: OK
    Running ‘spelling.R’
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘spelling.R’
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Differences:
      `actual`: -0.155 -0.014 0.990
    `expected`: -0.170 -0.000 0.990
    
    ── Failure ('test-Poisson_Regression.R:95:5'): Checking pois strata default values ──
    Expected `poisres$beta_0` to equal `c(-0.2431597, -1.9673368)`.
    Differences:
      `actual`: -0.134 -1.979
    `expected`: -0.243 -1.967
    
    
    [ FAIL 147 | WARN 0 | SKIP 15 | PASS 697 ]
    Error:
    ! Test failures.
    Execution halted
```
