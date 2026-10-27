# VSURF 1.2.2

Latest run: 2026-10-27: https://github.com/r-devel/linux-arm64-checks/actions/runs/40543981922

```
Package: VSURF
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    ── Failure ('test_orange.R:70:5'): Thresholds for the 3 steps ──────────────────
    Expected `orange.vsurf$sd.min` to equal 16.85953.
    Differences:
    1/1 mismatches
    [1] 19 - 16.9 == 2.13
    ── Failure ('test_orange.R:71:5'): Thresholds for the 3 steps ──────────────────
    Expected `orange.vsurf$mean.jump` to equal 331.2949.
    Differences:
    1/1 mismatches
    [1] 327 - 331 == -3.81
    
    [ FAIL 8 | WARN 1 | SKIP 0 | PASS 25 ]
    Error:
    ! Test failures.
    Execution halted

```
