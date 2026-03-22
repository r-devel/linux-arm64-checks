# ECOSolveR 0.6.1

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411328649

```
Package: ECOSolveR
Check: tests

AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    [ FAIL 1 | WARN 0 | SKIP 0 | PASS 82 ]
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test-bb.R:155:5'): test4 returns the right answer ─────────────────
    Expected `c(0, 0, 1, 1, 1, 0)` to equal `retval$x`.
    Differences:
    3/6 mismatches (average diff: 1)
    [1] 0 - 1.00e+00 == -1
    [3] 1 - 1.27e-10 ==  1
    [5] 1 - 4.58e-10 ==  1
    
    [ FAIL 1 | WARN 0 | SKIP 0 | PASS 82 ]
    Error:
    ! Test failures.
    Execution halted
```
