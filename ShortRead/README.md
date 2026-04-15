# ShortRead 1.69.3-2

Latest run: 2026-04-15: https://github.com/r-devel/linux-arm64-checks/actions/runs/24459722935

```
Package: ShortRead
Check: tests
AMD64: OK
    Running ‘ShortRead_unit_tests.R’
ARM64: ERROR
    Running ‘ShortRead_unit_tests.R’
  Running the tests in ‘tests/ShortRead_unit_tests.R’ failed.
  Last 13 lines of output:
     
    
    Test files with failing tests
    
       test_readPrb.R 
         test_readPrb_consistent 
         test_readPrb_input 
    
    
    Error in BiocGenerics:::testPackage("ShortRead") : 
      unit tests failed for package ShortRead
    In addition: Warning message:
    In for (i in seq_len(n)) { :
      closing unused connection 3 (/tmp/Rtmpfq8xiN/file1e456bc22ba5)
    Execution halted

```
