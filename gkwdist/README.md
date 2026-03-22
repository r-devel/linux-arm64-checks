# gkwdist 1.1.2

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411403782

```
Package: gkwdist
Check: tests

AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test-mle-performance.R:264:7'): Optimization efficiency for family: gkw ──
    Expected gkw_cfg1 : Analytical gradient precision is significantly worse <= `bench_result$none$mean_error * 2`.
    Actual comparison: 4.24 > 3.31
    Difference: 0.93 > 0
    Backtrace:
        ▆
     1. └─gkwdist (local) expect_efficiency_gain(bench, paste0(fam, "_cfg", cfg)) at test-mle-performance.R:264:7
     2.   └─testthat::expect_lte(...) at test-mle-performance.R:239:5
    
    [ FAIL 1 | WARN 0 | SKIP 0 | PASS 341 ]
    Error:
    ! Test failures.
    Execution halted
```
