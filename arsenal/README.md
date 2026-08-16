# arsenal 3.7.1

Latest run: 2026-08-16: https://github.com/r-devel/linux-arm64-checks/actions/runs/31918319965

```
Package: arsenal
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
      'test_write2.R:126:3', 'test_write2.R:131:3', 'test_write2.R:137:3',
      'test_write2.R:192:3'
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test_lhs_modelsum.R:19:3'): A modelsum call with strata ───────────
    Expected `capture.kable(...)` to be identical to `c(...)`.
    Differences:
    1/20 mismatches
    x[5]: "|      |Treatment Arm B |-1.813   |2.331     |0.444   |              |"
    y[5]: "|      |Treatment Arm B |-1.812   |2.331     |0.444   |              |"
    
    [ FAIL 1 | WARN 0 | SKIP 12 | PASS 499 ]
    Error:
    ! Test failures.
    Execution halted

```
