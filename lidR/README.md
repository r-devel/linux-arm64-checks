# lidR 4.2.3

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411479842

```
Package: lidR
Check: examples

AMD64: OK
ARM64: ERROR
  Running examples in ‘lidR-Ex.R’ failed
  The error most likely occurred in:
  
  > ### Name: Extract
  > ### Title: Extract or Replace Parts of a LAS* Object
  > ### Aliases: Extract $,LAS-method [[,LAS,ANY,missing-method $<-,LAS-method
  > ###   [[<-,LAS,ANY,missing-method [,LAS,numeric,ANY-method
  > ###   [,LAS,logical,ANY-method [,LAS,sf,ANY-method [,LAS,sfc,ANY-method
  > ###   $,LAScatalog-method [[,LAScatalog,ANY,missing-method
  > ###   [,LAScatalog,ANY,ANY-method [,LAScatalog,logical,ANY-method
  > ###   [,LAScatalog,sf,ANY-method [,LAScatalog,sfc,ANY-method
  > ###   [[<-,LAScatalog,ANY,ANY-method $<-,LAScatalog-method
  > ###   $,LASheader-method $<-,LASheader-method
  > ###   [[,LASheader,ANY,missing-method
  > ###   [[<-,LASheader,character,missing-method
  > 
  > ### ** Examples
  > 
  > LASfile <- system.file("extdata", "example.laz", package="rlas")
  > las = readLAS(LASfile)
  
                                                                                  
  Error: Invalid data: ScanAngleRank is not an unsigned integer on 8 bits
  Execution halted
Package: lidR
Check: tests

AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
     13. │                     └─base::eval(exprs, env)
     14. │                       ├─lidR::readLAS(megaplot_laz_path) at ./setup-testthat.R:20:1
     15. │                       └─lidR:::readLAS.character(megaplot_laz_path)
     16. │                         ├─lidR:::streamLAS(files, ofile = "", select, filter)
     17. │                         └─lidR:::streamLAS.character(files, ofile = "", select, filter)
     18. │                           └─lidR::LAS(data, header, check = TRUE, index = NULL, no_attr_name_check = TRUE)
     19. │                             └─rlas::is_valid_ScanAngleRank(data, "stop")
     20. │                               └─rlas:::is_no_na_integer_on_n_bits(...)
     21. │                                 └─rlas:::error_handling_engine(errors, behavior)
     22. │                                   └─base::stop(errors[1], call. = FALSE)
     23. └─base::.handleSimpleError(...)
     24.   └─testthat (local) h(simpleError(msg, call))
     25.     └─cli::cli_abort(...)
     26.       └─rlang::abort(...)
    Execution halted
```
