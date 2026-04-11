# pam 2.1.1

Latest run: 2026-04-11: https://github.com/r-devel/linux-arm64-checks/actions/runs/24289527713

```
Package: pam
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Differences:
      `actual`: -0.018109014
    `expected`: -0.018109015
    
    ── Failure ('test-walsby_etr_II.R:54:3'): test-walsby_etr_II generate regression modified 20240925.csv - linux ──
    Expected `model_result[["beta"]]` to equal `-0.018109015`.
    Differences:
      `actual`: -0.018109014
    `expected`: -0.018109015
    
    
    [ FAIL 108 | WARN 0 | SKIP 0 | PASS 1035 ]
    Error:
    ! Test failures.
    Execution halted

```
