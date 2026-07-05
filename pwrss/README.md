# pwrss 1.2.0

Latest run: 2026-07-05: https://github.com/r-devel/linux-arm64-checks/actions/runs/28727116379

```
Package: pwrss
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Differences:
    `actual$comparison`:   "A2 A3 <=> A1"
    `expected$comparison`: "A3 <=> A1"   
    
    ── Failure ('test-ancova.R:755:5'): power.f.ancova.shieh / power.t.contrasts / power.t.contrast work ──
    Expected `...[]` to equal `list(...)`.
    Differences:
    `actual$comparison`:   "A2 A3 <=> A1" "A1 A3 <=> A2"
    `expected$comparison`: "A3 <=> A1"    "A1 A3 <=> A2"
    
    
    [ FAIL 3 | WARN 0 | SKIP 1 | PASS 2422 ]
    Error:
    ! Test failures.
    Execution halted

```
