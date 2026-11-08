# LiblineaR 2.50-1

Latest run: 2026-11-08: https://github.com/r-devel/linux-arm64-checks/actions/runs/42474558779

```
Package: LiblineaR
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    - actual[7, ]     2.1013190  2.46801166 -7.6955939
    + expected[7, ]   2.1612050 -0.59837205 -7.7304402
    - actual[8, ]     1.8311734  2.36807952 -7.4729769
    + expected[8, ]   1.8912765 -0.59268294 -7.5089902
    - actual[9, ]     2.2211633  2.19953868 -6.6690286
    + expected[9, ]   2.2807850 -0.73698152 -6.7180692
    - actual[10, ]    2.1303098  2.57519928 -8.0728386
    + expected[10, ]  2.1910330 -0.57390537 -8.1038890
    and 50 more ...
    
    
    [ FAIL 9 | WARN 0 | SKIP 1 | PASS 2153 ]
    Error:
    ! Test failures.
    Execution halted

```
