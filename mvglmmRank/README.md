# mvglmmRank 1.2-6

Latest run: 2026-09-18: https://github.com/r-devel/linux-arm64-checks/actions/runs/35393924407

```
Package: mvglmmRank
Check: tests
AMD64: OK
    Running ‘neutral-site-home-field.R’
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘neutral-site-home-field.R’
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    > test_check("mvglmmRank")
    Saving _problems/test-numerics-5.R
    [ FAIL 1 | WARN 0 | SKIP 0 | PASS 582 ]
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test-numerics.R:4:5'): probit derivatives agree with independent differentiation, including the tail ──
    Expected `.probit_derivative(q, order)` to equal `numDeriv::grad(...)`.
    Differences:
    actual != expected but don't know how to show the difference
    
    
    [ FAIL 1 | WARN 0 | SKIP 0 | PASS 582 ]
    Error:
    ! Test failures.
    Execution halted

```
