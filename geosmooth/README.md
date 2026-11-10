# geosmooth 0.2.0

Latest run: 2026-11-10: https://github.com/r-devel/linux-arm64-checks/actions/runs/42902333184

```
Package: geosmooth
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    • No source tree in installed checks. (1): 'test-neighbor-documentation.R:3:5'
    • package source tree is unavailable in installed-package tests (4):
      'test-exported-examples.R:3:5', 'test-ge0-skeleton.R:3:5',
      'test-geosmooth-native-naming.R:3:5', 'test-synthetic-guardrails.R:13:3'
    • source-tree test runner is not included in the package tarball (1):
      'test-test-runner-contract.R:3:3'
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test-logistic-trend-filtering.R:116:5'): invalid inputs and excessive dense workspace are rejected ──
    Expected `fit.logistic.trend.filtering(...)` to throw a error.
    
    [ FAIL 1 | WARN 0 | SKIP 6 | PASS 8689 ]
    Error:
    ! Test failures.
    Execution halted

```
