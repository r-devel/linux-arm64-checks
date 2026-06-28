# bootmlm 0.1.1

Latest run: 2026-06-28: https://github.com/r-devel/linux-arm64-checks/actions/runs/28309235528

```
Package: bootmlm
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Saving _problems/test-vcov-21.R
    [ FAIL 1 | WARN 53 | SKIP 0 | PASS 284 ]
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test-vcov.R:21:3'): vcov_vc() gives reasonable estimates as parametric bootstrap ──
    Expected `all(abs(log(sd_vc1/sd_vc1_lme)) < 0.1)` to be TRUE.
    Differences:
    `actual`:   FALSE
    `expected`: TRUE 
    
    
    [ FAIL 1 | WARN 53 | SKIP 0 | PASS 284 ]
    Error:
    ! Test failures.
    Execution halted

```
