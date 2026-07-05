# baggr 0.8.2

Latest run: 2026-07-05: https://github.com/r-devel/linux-arm64-checks/actions/runs/28726786659

```
Package: baggr
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    • On CRAN (8): 'test_binary.R:357:3', 'test_binary.R:415:3',
      'test_binary.R:444:3', 'test_full.R:4:1', 'test_loo.R:49:3',
      'test_multiarm.R:4:1', 'test_rubin.R:393:3', 'test_rubin.R:413:3'
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test_rubin.R:154:3'): Pooling metrics ─────────────────────────────
    Expected `as.numeric(pp[2, 1, 1])` to equal 0.75.
    Differences:
    1/1 mismatches
    [1] 0.627 - 0.75 == -0.123
    
    [ FAIL 1 | WARN 0 | SKIP 8 | PASS 664 ]
    Error:
    ! Test failures.
    Execution halted

```
