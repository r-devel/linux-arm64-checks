# ecoregime 0.3.1

Latest run: 2026-07-12: https://github.com/r-devel/linux-arm64-checks/actions/runs/29176345386

```
Package: ecoregime
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
      'test-plot.R:89:3', 'test-plot.R:107:3', 'test-plot.R:122:3',
      'test-plot.R:140:3'
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test-dist_edr.R:142:3'): the properties of dDR are fit ────────────
    Expected `dEDR[5, 3]` to equal 0.
    Differences:
      `actual`: 0.000000020
    `expected`: 0.000000000
    
    
    [ FAIL 1 | WARN 0 | SKIP 15 | PASS 276 ]
    Error:
    ! Test failures.
    Execution halted

```
