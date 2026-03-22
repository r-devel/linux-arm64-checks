# minimaxApprox 0.5.0

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411545666

```
Package: minimaxApprox
Check: tests

AMD64: OK
    Running ‘tinytest.R’
ARM64: ERROR
    Running ‘tinytest.R’
  Running the tests in ‘tests/tinytest.R’ failed.
  Last 13 lines of output:
    test_shared.R.................   20 tests [0;32mOK[0m 
    test_shared.R.................   20 tests [0;32mOK[0m 
    test_shared.R.................   21 tests [0;32mOK[0m 
    test_shared.R.................   21 tests [0;32mOK[0m 
    test_shared.R.................   22 tests [0;32mOK[0m 
    test_shared.R.................   22 tests [0;32mOK[0m 
    test_shared.R.................   22 tests [0;32mOK[0m 
    test_shared.R.................   23 tests [0;32mOK[0m 
    test_shared.R.................   24 tests [0;32mOK[0m 
    test_shared.R.................   25 tests [0;32mOK[0m [0;36m47ms[0m
    ----- FAILED[xcpt]: test_MiniMaxApprox.R<136--136>
     call| expect_warning(minimaxApprox(fn, -1, 1, 21, opts = opts), wrnMess)
     diff| No warning was emitted
    Error: 1 out of 141 tests failed
    Execution halted
```
