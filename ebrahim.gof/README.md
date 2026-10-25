# ebrahim.gof 2.10.0

Latest run: 2026-10-25: https://github.com/r-devel/linux-arm64-checks/actions/runs/40154899785

```
Package: ebrahim.gof
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    ── Failure ('test-localize.R:170:3'): naming = 'holm' and 'bonferroni' reproduce the paper's script ──
    Expected `rb$adjusted` to equal `c(INTERCEPT = 0.44, SLOPE = 0.36, LINK = 0.16, COV = 0.04)`.
    Differences:
    1/4 mismatches
    [1] 0.4 - 0.44 == -0.04
    ── Failure ('test-localize.R:184:3'): robust = TRUE reproduces the paper's script ──
    Expected `unname(...)` to equal `c(0.11, 0.07, 0.04, 0.01, 0.02)`.
    Differences:
    1/5 mismatches
    [1] 0.1 - 0.11 == -0.01
    
    [ FAIL 4 | WARN 31 | SKIP 14 | PASS 1044 ]
    Error:
    ! Test failures.
    Execution halted

```
