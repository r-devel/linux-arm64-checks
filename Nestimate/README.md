# Nestimate 0.8.0

Latest run: 2026-07-26: https://github.com/r-devel/linux-arm64-checks/actions/runs/30183750813

```
Package: Nestimate
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    • Source-tree introspection test: hypa.R not present in install (2):
      'test-fix-FIX5.R:47:3', 'test-fix-FIX5.R:77:3'
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test-mcml_pc.R:719:3'): lavaan arguments pass through ... verbatim ──
    Expected `identical(f_wlsmv$loadings$weight, f_ulsmv$loadings$weight)` to be FALSE.
    Differences:
    `actual`:   TRUE 
    `expected`: FALSE
    
    
    [ FAIL 1 | WARN 64 | SKIP 33 | PASS 4255 ]
    Error:
    ! Test failures.
    Execution halted

```
