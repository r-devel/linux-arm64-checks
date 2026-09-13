# HDElliptical 0.1.2

Latest run: 2026-09-13: https://github.com/r-devel/linux-arm64-checks/actions/runs/34732399926

```
Package: HDElliptical
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Differences:
      `actual`: 0.0
    `expected`: 1.0
    
    ── Failure ('test-chapter2-pdq-sign.R:500:3'): U(0)=0 is limited to cross signs and fitted zeros fail ──
    Expected `unname(cross.zero$components$cross.signs$group1[5L, ])` to equal `c(0, 0, 0)`.
    Differences:
      `actual`: 0.0 0.0 -1.0
    `expected`: 0.0 0.0  0.0
    
    
    [ FAIL 3 | WARN 0 | SKIP 0 | PASS 6255 ]
    Error:
    ! Test failures.
    Execution halted

```
