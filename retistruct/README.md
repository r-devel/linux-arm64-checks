# retistruct 0.8.1

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411728379

```
Package: retistruct
Check: tests

AMD64: OK
    Running ‘spelling.R’
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘spelling.R’
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Backtrace:
        ▆
     1. └─a$triangulate(suppress.external.steiner = TRUE) at test-stitched-outline.R:293:3
     2.   └─TriangulatedFragment$new(...)
     3.     └─retistruct (local) initialize(...)
     4.       └─RTriangle::triangulate(...)
    
    [ FAIL 5 | WARN 0 | SKIP 4 | PASS 288 ]
    Error:
    ! Test failures.
    Warning messages:
    1: In rgl.init(initValue, onlyNULL) : RGL: unable to open X11 display
    2: 'rgl.init' failed, will use the null device.
    See '?rgl.useNULL' for ways to avoid this warning. 
    Execution halted
```
