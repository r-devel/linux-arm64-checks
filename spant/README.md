# spant 4.0.0

Latest run: 2026-05-17: https://github.com/r-devel/linux-arm64-checks/actions/runs/25979403830

```
Package: spant
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    [ FAIL 1 | WARN 0 | SKIP 0 | PASS 16 ]
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test_qm_sim.R:11:3'): LCM .basis files can be written and read back ──
    `basis_read` has changed from known value recorded in 'def_basis.rds'.
    Component "data": Mean relative Mod difference: 1.035276e-06
    Backtrace:
        ▆
     1. └─testthat::expect_equal_to_reference(...) at test_qm_sim.R:11:3
     2.   └─testthat::expect_known_value(..., update = update)
    
    [ FAIL 1 | WARN 0 | SKIP 0 | PASS 16 ]
    Error:
    ! Test failures.
    Execution halted

```
