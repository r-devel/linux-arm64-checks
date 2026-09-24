# psvr 0.1.0

Latest run: 2026-09-24: https://github.com/r-devel/linux-arm64-checks/actions/runs/36046475346

```
Package: psvr
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    [58] 0.0133350773907 | 0.0133350773907 [58]           
    [59] 0.0105448879339 - 0.0101626247096 [59]           
    [60] 0.0094235783803 - 0.0105236996638 [60]           
    [61] 0.0092592683582 - 0.0087278515739 [61]           
    [62] 0.0079099220777 - 0.0070684250184 [62]           
    [63] 0.0081565942326 - 0.0073471992161 [63]           
    [64] 0.0078367618973 - 0.0076212975542 [64]           
    [65] 0.0079903669579 - 0.0090402817024 [65]           
     ... ...               ...             and 17 more ...
    
    
    [ FAIL 4 | WARN 2 | SKIP 70 | PASS 893 ]
    Error:
    ! Test failures.
    Execution halted

```
