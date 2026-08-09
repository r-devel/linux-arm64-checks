# lorax 0.1.0

Latest run: 2026-08-09: https://github.com/r-devel/linux-arm64-checks/actions/runs/31288078242

```
Package: lorax
Check: tests
AMD64: OK
    Running ‘spelling.R’
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘spelling.R’
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    • Skipping (1): 'test-cforest.R:2:1'
    • TOOOO LONG (1): 'test-party.R:1:1'
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test-ObliqueForest.R:316:5'): extract_rules.ObliqueForest() node assignments are consistent ──
    Expected `obs_in_node_aorsf` to have the same values as `obs_in_node_rule`.
    Actual: 3, 65, 99, 127, 144
    Expected: 3, 65, 127, 134, 144
    Needs: 99
    Absent: 134
    
    [ FAIL 1 | WARN 0 | SKIP 71 | PASS 1411 ]
    Error:
    ! Test failures.
    Execution halted

```
