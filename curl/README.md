# curl 8.1.0

Latest run: 2026-10-14: https://github.com/r-devel/linux-arm64-checks/actions/runs/38615824145

```
Package: curl
Check: package dependencies
AMD64: OK
ARM64: WARNING
  Cannot process vignettes
  Packages suggested but not available for checking:
    'spelling', 'testthat', 'knitr', 'jsonlite', 'later', 'rmarkdown',
    'httpuv', 'webutils'
  
  VignetteBuilder package required for checking but not installed: ‘knitr’

Package: curl
Check: tests
AMD64: OK
    Running ‘spelling.R’
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘spelling.R’
    Comparing ‘spelling.Rout’ to ‘spelling.Rout.save’ ...
  5a6
  > All Done!
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Complete output:
    > library(testthat)
    Error in library(testthat) : there is no package called 'testthat'
    Execution halted

```
