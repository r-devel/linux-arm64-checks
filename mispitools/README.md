# mispitools 2.0.0

Latest run: 2026-08-25: https://github.com/r-devel/linux-arm64-checks/actions/runs/32906993078

```
Package: mispitools
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
     2.   └─testthat::expect_equal(cpp$p_h1, ref$p_h1, tolerance = tol, info = info) at test-per-marker-lr-dist-cpp.R:28:3
    ── Failure ('test-per-marker-lr-dist-cpp.R:174:3'): cpp_per_marker_lr_dist matches R-ref on trio K=4 mut=stepwise ──
    Expected `cpp$p_h2` to equal `ref$p_h2`.
    Differences:
    Lengths differ: 522 is not 520
    trio K=4 mut=stepwise
    Backtrace:
        ▆
     1. └─mispitools (local) expect_lrdist_equal(cpp, ref, info = "trio K=4 mut=stepwise") at test-per-marker-lr-dist-cpp.R:174:3
     2.   └─testthat::expect_equal(cpp$p_h2, ref$p_h2, tolerance = tol, info = info) at test-per-marker-lr-dist-cpp.R:29:3
    
    [ FAIL 23 | WARN 0 | SKIP 23 | PASS 2446 ]
    Error:
    ! Test failures.
    Execution halted

```
