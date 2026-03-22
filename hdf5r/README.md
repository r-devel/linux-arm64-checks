# hdf5r 1.3.12

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411435381

```
Package: hdf5r
Check: tests

AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    
        error #001: ../../../src/H5Tenum.c in H5T__enum_insert(): line 190: value redefinition
            class: HDF5
            major: Datatype
            minor: Unable to initialize object
    
    Backtrace:
        ▆
     1. └─H5T_ENUM$new(...) at test-convert.R:108:5
     2.   └─hdf5r (local) initialize(...)
    
    [ FAIL 1 | WARN 0 | SKIP 3 | PASS 982 ]
    Error:
    ! Test failures.
    Execution halted
```
