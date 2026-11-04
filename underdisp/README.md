# underdisp 0.2.0

Latest run: 2026-11-04: https://github.com/r-devel/linux-arm64-checks/actions/runs/41927779544

```
Package: underdisp
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
      'test-zi-offset.R:7:3', 'test-zi-offset.R:23:3', 'test-zi-offset.R:36:3',
      'test-zi-separation.R:19:3', 'test-zi-separation.R:106:3', 'test-zi.R:2:3'
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test-newdata-units.R:143:3'): dispersion_test()'s fixed-effects null does not depend on centring a covariate ──
    Expected `unname(t1$statistic)` to equal `unname(t2$statistic)`.
    Differences:
      `actual`: 0.8794432
    `expected`: 0.8794446
    
    
    [ FAIL 1 | WARN 5 | SKIP 100 | PASS 732 ]
    Error:
    ! Test failures.
    Execution halted

```
