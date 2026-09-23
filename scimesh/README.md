# scimesh 0.4.0

Latest run: 2026-09-23: https://github.com/r-devel/linux-arm64-checks/actions/runs/35802078986

```
Package: scimesh
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    + expected[13, ] -0.80000001  0.000000e+00 -0.6000000
      actual[14, ]   -0.88022882  3.904344e-01 -0.2697372
      actual[15, ]   -0.72460109  6.762523e-01  0.1328015
      actual[16, ]   -0.37481701  7.808688e-01  0.4997561
      actual[17, ]    0.07539897  6.762522e-01  0.7328015
      actual[18, ]    0.50541180  3.904345e-01  0.7694933
    - actual[19, ]    0.80000007 -6.268505e-08  0.6000000
    + expected[19, ]  0.80000007 -6.826572e-08  0.6000000
    and 3 more ...
    
    
    [ FAIL 1 | WARN 0 | SKIP 0 | PASS 689 ]
    Error:
    ! Test failures.
    Execution halted

```
