# metaSEM 2.0

Latest run: 2026-11-22: https://github.com/r-devel/linux-arm64-checks/actions/runs/44967010281

```
Package: metaSEM
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    ── Failure ('test_review_fixes.R:182:3'): unit variances hold at each moderator pattern ──
    `osmasem2(...)` produced unexpected warnings.
    Expected match: no basis
    Actual values:
    * constraint-adjusted standard errors could not be calculated because the coefficient matrix of the quadratic form was uninvertible
    ── Failure ('test_review_fixes.R:191:3'): unit variances hold at each moderator pattern ──
    `osmasem2(...)` produced unexpected warnings.
    Expected match: no basis
    Actual values:
    * constraint-adjusted standard errors could not be calculated because the coefficient matrix of the quadratic form was uninvertible
    
    [ FAIL 4 | WARN 3 | SKIP 36 | PASS 1549 ]
    Error:
    ! Test failures.
    Execution halted

```
