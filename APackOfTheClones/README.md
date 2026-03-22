# APackOfTheClones 1.3.0

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411218902

```
Package: APackOfTheClones
Check: tests

AMD64: OK
    Running ‘spelling.R’
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘spelling.R’
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    [10] -7.224835 | -7.224835  [10]           
    [11] -0.749929 - -0.352190  [11]           
    [12] -0.153764 - -0.952277  [12]           
    [13] 0.445213  - 0.446534   [13]           
    [14] -1.063389 - -0.048439  [14]           
    [15] -0.467224 - -0.648526  [15]           
    [16] 0.810954  - 0.924517   [16]           
    [17] 0.131753  - -1.247324  [17]           
     ... ...         ...        and 25 more ...
    
    
    [ FAIL 1 | WARN 0 | SKIP 15 | PASS 244 ]
    Error:
    ! Test failures.
    Execution halted
```
