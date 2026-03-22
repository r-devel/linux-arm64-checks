# memuse 4.2-3

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411531658

```
Package: memuse
Check: tests

AMD64: OK
    Running ‘accessors.R’
    Running ‘arithmetic.R’
    Running ‘comparators.R’
    Running ‘constructor.R’
    Running ‘converters.r’
    Running ‘howbig.R’
    Running ‘howmany.r’
    Running ‘hr.R’
    Running ‘swap.R’
    Running ‘sysinfo.R’
ARM64: ERROR
    Running ‘accessors.R’
    Running ‘arithmetic.R’
    Running ‘comparators.R’
    Running ‘constructor.R’
    Running ‘converters.r’
    Running ‘howbig.R’
    Running ‘howmany.r’
    Running ‘hr.R’
    Running ‘swap.R’
    Running ‘sysinfo.R’
  Running the tests in ‘tests/sysinfo.R’ failed.
  Last 13 lines of output:
    > # is running this. So we settle for ensuring evaluation without error.
    > iswin <- function() tolower(.Platform$OS.type) == "windows"
    > ismac <- function() tolower(as.character(Sys.info()["sysname"])) == "darwin"
    > islin <- function() tolower(as.character(Sys.info()["sysname"])) == "linux"
    > supported = function() iswin() || ismac() || islin()
    > 
    > if (supported()){
    +   invisible(Sys.meminfo())
    +   invisible(Sys.swapinfo())
    +   invisible(Sys.procmem())
    +   invisible(Sys.cachesize())
    +   invisible(Sys.cachelinesize())
    + }
    Error in Sys.cachesize() : platform not supported at this time
    Execution halted
```
