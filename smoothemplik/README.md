# smoothemplik 0.0.17

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411799243

```
Package: smoothemplik
Check: tests

AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    ══ Skipped tests (1) ═══════════════════════════════════════════════════════════
    • empty test (1):
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test-svdlm.R:27:3'): LM via SVD works and recovers from failures ──
    Expected `svdlm(1:10, 1:10)` to be identical to 1.
    Differences:
      `actual`: 0.99999999999999978
    `expected`: 1.00000000000000000
    
    
    [ FAIL 1 | WARN 0 | SKIP 1 | PASS 253 ]
    Error:
    ! Test failures.
    Execution halted
```
