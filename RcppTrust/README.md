# RcppTrust 0.2.0

Latest run: 2026-10-27: https://github.com/r-devel/linux-arm64-checks/actions/runs/40542292967

```
Package: RcppTrust
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    ── Failure ('test-minqa.R:68:5'): bobyqa() matches minqa::bobyqa() exactly ─────
    Expected `ours$par` to equal `theirs$par`.
    Differences:
      `actual`: 0.06688 0.36668 0.28874 0.63332 0.71126 0.93312
    `expected`: 0.06688 0.28874 0.36668 0.63332 0.71126 0.93312
    
    Backtrace:
        ▆
     1. └─RcppTrust (local) expectSameAsMinqa(ours, theirs, wellPosed = !isFALSE(cs$wellPosed)) at test-minqa.R:68:5
     2.   └─testthat::expect_equal(ours$par, theirs$par, tolerance = 1e-04) at test-minqa.R:44:5
    
    [ FAIL 1 | WARN 0 | SKIP 2 | PASS 248 ]
    Error:
    ! Test failures.
    Execution halted

```
