# retistruct 0.8.1

Latest run: 2026-05-17: https://github.com/r-devel/linux-arm64-checks/actions/runs/25979309315

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

Package: retistruct
Check: whether package can be installed
AMD64: WARNING
  Found the following significant warnings:
    Warning: 'rgl.init' failed, will use the null device.
  See ‘/__w/linux-arm64-checks/linux-arm64-checks/retistruct.Rcheck/00install.out’ for details.
  Used C compiler: ‘x86_64-linux-gnu-gcc (Ubuntu 15.2.0-16ubuntu1) 15.2.0’
ARM64: WARNING
  Found the following significant warnings:
    Warning: 'rgl.init' failed, will use the null device.
  See ‘/__w/linux-arm64-checks/linux-arm64-checks/retistruct.Rcheck/00install.out’ for details.
  Used C compiler: ‘aarch64-linux-gnu-gcc (Ubuntu 15.2.0-16ubuntu1) 15.2.0’

```
