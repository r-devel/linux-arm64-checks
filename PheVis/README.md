# PheVis 1.0.5

Latest run: 2026-10-30: https://github.com/r-devel/linux-arm64-checks/actions/runs/40989070235

```
Package: PheVis
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    > test_check("PheVis")
    Saving _problems/test-traintest_phevis-53.R
    [ FAIL 1 | WARN 21 | SKIP 0 | PASS 3 ]
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test-traintest_phevis.R:53:9'): test all pipeline is working ──────
    Expected `check_value[2]` to equal 0.
    Differences:
    1/1 mismatches
    [1] -0.0103 - 0 == -0.0103
    
    [ FAIL 1 | WARN 21 | SKIP 0 | PASS 3 ]
    Error:
    ! Test failures.
    Execution halted

```
