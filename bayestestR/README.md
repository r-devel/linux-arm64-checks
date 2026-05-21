# bayestestR 0.18.0

Latest run: 2026-05-21: https://github.com/r-devel/linux-arm64-checks/actions/runs/26250781869

```
Package: bayestestR
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
      'test-describe_posterior.R:145:3', 'test-weighted_posteriors.R:1:1'
    • TODO: check hard-coded values (1): 'test-check_prior.R:29:3'
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test-diagnostic_posterior.R:29:3'): diagnostic_posterior default ──
    Expected `dp2$Rhat` to equal `c(1.00125536330078, 1.00087301991599)`.
    Differences:
      `actual`: 1.001255 1.000845
    `expected`: 1.001255 1.000873
    
    
    [ FAIL 1 | WARN 0 | SKIP 81 | PASS 265 ]
    Error:
    ! Test failures.
    Execution halted

```
