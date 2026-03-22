# crownsegmentr 1.0.1

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411295610

```
Package: crownsegmentr
Check: tests

AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
        ▆
     1. ├─lidR::clip_rectangle(...) at test-watershed_diameter_raster.R:11:3
     2. ├─lidR::readLAS(test_point_cloud_file_path)
     3. └─lidR:::readLAS.character(test_point_cloud_file_path)
     4.   ├─lidR:::streamLAS(files, ofile = "", select, filter)
     5.   └─lidR:::streamLAS.character(files, ofile = "", select, filter)
     6.     └─lidR::LAS(data, header, check = TRUE, index = NULL, no_attr_name_check = TRUE)
     7.       └─rlas::is_valid_ScanAngleRank(data, "stop")
     8.         └─rlas:::is_no_na_integer_on_n_bits(...)
     9.           └─rlas:::error_handling_engine(errors, behavior)
    
    [ FAIL 6 | WARN 0 | SKIP 3 | PASS 33 ]
    Error:
    ! Test failures.
    Execution halted
```
