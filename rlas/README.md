# rlas 1.8.4

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411731980

```
Package: rlas
Check: tests

AMD64: OK
    Running ‘tinytest.R’
ARM64: ERROR
    Running ‘tinytest.R’
  Running the tests in ‘tests/tinytest.R’ failed.
  Last 13 lines of output:
    test_altrep.R.................   43 tests [0;32mOK[0m 
    test_altrep.R.................   44 tests [0;32mOK[0m 
    test_altrep.R.................   45 tests [0;32mOK[0m [0;36m4ms[0m
    
    test-altrep_iolas.R...........    0 tests    
    test-altrep_iolas.R...........    0 tests    
                                                                                    
    
    test-altrep_iolas.R...........    0 tests    
    test-altrep_iolas.R...........    0 tests    
    test-altrep_iolas.R...........    1 tests [0;32mOK[0m 
    test-altrep_iolas.R...........    2 tests [0;32mOK[0m 
    test-altrep_iolas.R...........    3 tests [0;32mOK[0m 
    test-altrep_iolas.R...........    4 tests [0;32mOK[0m Error: Invalid data: ScanAngleRank is not an unsigned integer on 8 bits
    Execution halted
```
