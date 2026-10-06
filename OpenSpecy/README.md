# OpenSpecy 2.0.1

Latest run: 2026-10-06: https://github.com/r-devel/linux-arm64-checks/actions/runs/37397121490

```
Package: OpenSpecy
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    • Repository-only workspace path contract is not in the package tarball (1):
      'test-shinylive_wasm.R:845:5'
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test-build_lib.R:913:3'): build_lib() runs default joins, processing, SNR, and assessment ──
    Expected `all(vapply(built, check_OpenSpecy, logical(1)))` to be TRUE.
    Differences:
    `actual`:   FALSE
    `expected`: TRUE 
    
    
    [ FAIL 1 | WARN 31 | SKIP 28 | PASS 3746 ]
    Error:
    ! Test failures.
    Execution halted

```
