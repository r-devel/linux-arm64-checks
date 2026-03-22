# mmap 0.6-24

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411560698

```
Package: mmap
Check: tests

AMD64: OK
    Running ‘integers.R’
ARM64: ERROR
    Running ‘integers.R’
  Running the tests in ‘tests/integers.R’ failed.
  Last 13 lines of output:
    +     cat("test.int32 disabled\n")
    +     return(NULL)
    +   }
    +   writeBin(0.0, tmp)
    +   m <- mmap(tmp, int64())  # signed 8 byte integers as doubles
    +   m[] <- 2^40
    +   if( !all(m[] == 2^40) )
    +     stop("m[] == 2^40")
    +   munmap(m)
    +   cat("OK\n")
    + }
    > 
    > test.int8()
    Error in test.int8() : m[] == (-128:127L)
    Execution halted
```
