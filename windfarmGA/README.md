# windfarmGA 5.0.0

Latest run: 2026-09-14: https://github.com/r-devel/linux-arm64-checks/actions/runs/34846821532

```
Package: windfarmGA
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Error ('test_ga.R:95:3'): Test Genetic Algorithm with different Inputs ──────
    Error in `grid_area(area, resol2, proportionality)`: A grid cannot be drawn. Reduce the `size` argument or define a projection in meters.
    Backtrace:
        ▆
     1. ├─windfarmGA (local) quiet(...) at test_ga.R:95:3
     2. │ └─base::force(x) at test_ga.R:6:3
     3. └─windfarmGA::genetic_algorithm(...)
     4.   └─windfarmGA::grid_area(area, resol2, proportionality)
    
    [ FAIL 1 | WARN 0 | SKIP 2 | PASS 834 ]
    Error:
    ! Test failures.
    Execution halted

```
