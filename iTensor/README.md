# iTensor 1.0.4

Latest run: 2026-05-08: https://github.com/r-devel/linux-arm64-checks/actions/runs/25559657810

```
Package: iTensor [Old version: 1.0.2, New version: 1.0.4]
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    [ FAIL 1 | WARN 0 | SKIP 0 | PASS 271 ]
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Error ('test-GroupICA.R:14:1'): (code run outside of `test_that()`) ─────────
    Error in `Gs[[i_group]] %*% A`: non-conformable arguments
    Backtrace:
        ▆
     1. └─iTensor::GroupICA(...) at test-GroupICA.R:14:1
     2.   └─iTensor:::.Calhoun2009(...)
     3.     └─MASS::ginv(Gs[[i_group]] %*% A)
    
    [ FAIL 1 | WARN 0 | SKIP 0 | PASS 271 ]
    Error:
    ! Test failures.
    Execution halted

```
