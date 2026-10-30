# jumps 2.0.0

Latest run: 2026-10-30: https://github.com/r-devel/linux-arm64-checks/actions/runs/41069575385

```
Package: jumps
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    > 
    > test_check("jumps")
    Saving _problems/test-ssj-186.R
    [ FAIL 1 | WARN 0 | SKIP 0 | PASS 404 ]
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test-ssj.R:186:3'): the default maxsum is the range of x, not the rescaled one ──
    Expected `sum(f$gamma)` <= `f$maxsum * (1 + 1e-08)`.
    Actual comparison: 3.3500011 > 3.3500000
    Difference: 0.0000011 > 0
    
    [ FAIL 1 | WARN 0 | SKIP 0 | PASS 404 ]
    Error:
    ! Test failures.
    Execution halted

```
