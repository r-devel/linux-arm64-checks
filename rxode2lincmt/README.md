# rxode2lincmt 0.1.0

Latest run: 2026-09-24: https://github.com/r-devel/linux-arm64-checks/actions/runs/36046833121

```
Package: rxode2lincmt
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    ── Failure ('test-dual.R:28:5'): linCmtModelDouble serves sensType 32 and agrees with 3 to round-off ──
    Expected `as.numeric(.a$val)` to be identical to `as.numeric(.b$val)`.
    Differences:
      `actual`: 3.01547218734179046
    `expected`: 3.01547218734179001
    
    ── Failure ('test-dual.R:29:5'): linCmtModelDouble serves sensType 32 and agrees with 3 to round-off ──
    Expected `.relMax(.a$J, .b$J)` < 1e-12.
    Actual comparison: 0.000000000024 >= 0.000000000001
    Difference: 0.000000000023 >= 0
    
    [ FAIL 2 | WARN 0 | SKIP 0 | PASS 131 ]
    Error:
    ! Test failures.
    Execution halted

```
