# normalblockr 0.3.0

Latest run: 2026-09-13: https://github.com/r-devel/linux-arm64-checks/actions/runs/34733210820

```
Package: normalblockr
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Saving _problems/test-ZINormalBlockMeanUnknownClusters-53.R
    [ FAIL 1 | WARN 72 | SKIP 0 | PASS 636 ]
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test-ZINormalBlockMeanUnknownClusters.R:53:3'): a collection over a range of q runs, selects and refines ──
    Expected `all(diff(coll$criteria$deviance) <= 1e-06)` to be TRUE.
    Differences:
    `actual`:   FALSE
    `expected`: TRUE 
    
    
    [ FAIL 1 | WARN 72 | SKIP 0 | PASS 636 ]
    Error:
    ! Test failures.
    Execution halted

```
