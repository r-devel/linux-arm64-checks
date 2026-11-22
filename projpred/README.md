# projpred 3.0.0

Latest run: 2026-11-22: https://github.com/r-devel/linux-arm64-checks/actions/runs/44967511518

```
Package: projpred
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Differences:
    8/11 mismatches (average diff: 2.41e-08)
    [1]  -0.0767 - -0.0767 == -1.43e-08
    [2]   0.5968 -  0.5968 ==  2.25e-08
    [3]   0.1457 -  0.1457 ==  2.18e-08
    [5]   0.1284 -  0.1284 ==  1.62e-08
    [7]   0.1296 -  0.1296 ==  1.95e-08
    [9]  -0.2987 - -0.2987 == -2.32e-08
    [10]  0.4502 -  0.4502 ==  4.73e-08
    [11] -0.3661 - -0.3661 == -2.82e-08
    
    [ FAIL 2 | WARN 3 | SKIP 249 | PASS 5219 ]
    Error:
    ! Test failures.
    Execution halted

```
