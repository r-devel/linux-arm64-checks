# vostokR 0.2.1

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23633682569

```
Package: vostokR
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Backtrace:
        ▆
     1. ├─lidR::readLAS(LASfile) at test-solar_potential.R:11:1
     2. └─lidR:::readLAS.character(LASfile)
     3.   ├─lidR:::streamLAS(files, ofile = "", select, filter)
     4.   └─lidR:::streamLAS.character(files, ofile = "", select, filter)
     5.     └─lidR::LAS(data, header, check = TRUE, index = NULL, no_attr_name_check = TRUE)
     6.       └─rlas::is_valid_ScanAngleRank(data, "stop")
     7.         └─rlas:::is_no_na_integer_on_n_bits(...)
     8.           └─rlas:::error_handling_engine(errors, behavior)
    
    [ FAIL 1 | WARN 0 | SKIP 0 | PASS 0 ]
    Error:
    ! Test failures.
    Execution halted

```
