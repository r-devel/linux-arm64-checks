# ivdtools 0.1.2

Latest run: 2026-08-23: https://github.com/r-devel/linux-arm64-checks/actions/runs/32609854328

```
Package: ivdtools
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Saving _problems/test-sensitivity-34.R
    [ FAIL 1 | WARN 0 | SKIP 0 | PASS 333 ]
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test-sensitivity.R:34:3'): full pipeline: LoB / LoD / LoQ match EP17-A2 and analytic values ──
    Expected `res$model` to equal "Model_4".
    Differences:
    `actual`:   "Model_8"
    `expected`: "Model_4"
    
    
    [ FAIL 1 | WARN 0 | SKIP 0 | PASS 333 ]
    Error:
    ! Test failures.
    Execution halted

```
