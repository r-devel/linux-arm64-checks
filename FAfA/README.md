# FAfA 1.4

Latest run: 2026-10-01: https://github.com/r-devel/linux-arm64-checks/actions/runs/36797218401

```
Package: FAfA
Check: tests
AMD64: OK
    Running ‘spelling.R’
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘spelling.R’
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Expected `result$m_values[, "m_pr_4rth_power"]` to equal `c(...)`.
    Differences:
        actual         | expected          
    [1] 10.31157803778 | 10.31157803778 [1]
    [2] 31.42205093515 | 31.42205093515 [2]
    [3] 0.54074987791  | 0.54074987791  [3]
    [4] 2.85561771510  - 2.85561771508  [4]
    [5] 6.74765415192  - 6.74765415189  [5]
    [6] 42.99999771621 - 42.99999761360 [6]
    
    
    [ FAIL 2 | WARN 0 | SKIP 2 | PASS 219 ]
    Error:
    ! Test failures.
    Execution halted

```
