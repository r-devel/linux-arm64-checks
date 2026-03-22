# quanteda.textmodels 0.9.10

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411678958

```
Package: quanteda.textmodels
Check: tests

AMD64: OK
    Running ‘spelling.R’
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘spelling.R’
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    ── Failure ('test-textmodel_lr.R:23:5'): the lr model works with binomal classification ──
    Expected `as.matrix(coef(tmod))` to equal `matrix(...)`.
    Differences:
    6/9 mismatches (average diff: 0.266)
    [1]   6.608 -   6.607 ==  0.001204
    [2]   0.577 -   0.578 == -0.000715
    [6] -12.219 - -12.043 == -0.176420
    [7]  -2.061 -  -2.237 ==  0.175858
    [8] -13.659 - -14.281 ==  0.622011
    [9]  -0.622 -   0.000 == -0.622497
    
    [ FAIL 1 | WARN 0 | SKIP 1 | PASS 243 ]
    Error:
    ! Test failures.
    Execution halted
```
