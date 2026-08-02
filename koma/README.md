# koma 0.3.1

Latest run: 2026-08-02: https://github.com/r-devel/linux-arm64-checks/actions/runs/30728510515

```
Package: koma
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    • plotly is installed; skipping missing-package test. (1): 'test-plot.R:111:3'
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test-mass.R:57:3'): multivariate_norm returns correct values with set seed for a
    specific covariance matrix ──
    Expected `withr::with_seed(7, multivariate_norm(n = 1, mu = mu, sigma = sigma))` to equal `expected_result`.
    Differences:
      `actual`:  1.3 3.6 4.1
    `expected`: -1.2 0.8 1.5
    
    
    [ FAIL 1 | WARN 0 | SKIP 42 | PASS 846 ]
    Error:
    ! Test failures.
    Execution halted

```
