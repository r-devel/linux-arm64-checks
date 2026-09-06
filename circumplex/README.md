# circumplex 2.0.0

Latest run: 2026-09-06: https://github.com/r-devel/linux-arm64-checks/actions/runs/34005859116

```
Package: circumplex
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
         actual              | expected                
    [31] 0.61117119421377364 | 0.61117119421377364 [31]
    [32] 0.91078176809097244 | 0.91078176809097244 [32]
    [33] 0.66613935870906527 | 0.66613935870906527 [33]
    [34] 0.64818464789574282 - 0.64818464789574293 [34]
    [35] 0.67873148696801089 - 0.67873148696801078 [35]
    [36] 0.29102462601925816 | 0.29102462601925816 [36]
    [37] 0.57816413499026653 | 0.57816413499026653 [37]
    [38] 0.39672329985007021 | 0.39672329985007021 [38]
    
    
    [ FAIL 2 | WARN 4 | SKIP 540 | PASS 2398 ]
    Error:
    ! Test failures.
    Execution halted

```
