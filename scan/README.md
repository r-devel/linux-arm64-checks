# scan 0.68.0

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23953814899

```
Package: scan
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Saving _problems/test-between_smd-13.R
    [ FAIL 1 | WARN 0 | SKIP 0 | PASS 96 ]
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test-between_smd.R:13:3'): between_smd returns sc_bcsmd with REML models and expected columns ──
    Expected `object_checksum(res_no_resid)` to equal "1260.1821".
    Differences:
    `actual`:   "1260.1820"
    `expected`: "1260.1821"
    
    
    [ FAIL 1 | WARN 0 | SKIP 0 | PASS 96 ]
    Error:
    ! Test failures.
    Execution halted

```
