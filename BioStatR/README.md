# BioStatR 4.1.1

Latest run: 2026-08-23: https://github.com/r-devel/linux-arm64-checks/actions/runs/32575712244

```
Package: BioStatR
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    • On CRAN (3): 'test_gg_qqplot_vdiffr.R:1:1', 'test_gg_qqplot_vdiffr.R:10:1',
      'test_panel_hist_vdiffr.R:1:1'
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test_binom_ci_values.R:55:5'): binom.ci handles edge cases x=0 and x=n (end) ──
    Expected `all(m0[, "Lower"] >= 0 & m0[, "Upper"] <= 1)` to be TRUE.
    Differences:
    `actual`:   FALSE
    `expected`: TRUE 
    
    
    [ FAIL 1 | WARN 0 | SKIP 3 | PASS 67 ]
    Error:
    ! Test failures.
    Execution halted

```
