# polykde 1.2.0

Latest run: 2026-07-25: https://github.com/r-devel/linux-arm64-checks/actions/runs/30174748788

```
Package: polykde
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    ══ Skipped tests (6) ═══════════════════════════════════════════════════════════
    • No tests for euler ridges, just visualizations (1): 'tests_euler.R:504:1'
    • Unstable (5): 'tests_kde.R:165:3', 'tests_kre.R:49:3', 'tests_tests.R:115:3',
      'tests_tests.R:191:3', 'tests_tests.R:200:3'
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('tests_tests.R:240:3'): Tests do not reject H_0 when it is true ────
    Expected `pval_mea` > 0.05.
    Actual comparison: 0.020 <= 0.050
    Difference: -0.030 <= 0
    
    [ FAIL 1 | WARN 0 | SKIP 6 | PASS 1045 ]
    Error:
    ! Test failures.
    Execution halted

```
