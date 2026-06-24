# migraph 1.6.2

Latest run: 2026-06-24: https://github.com/r-devel/linux-arm64-checks/actions/runs/28085708371

```
Package: migraph [Old version: 1.6.6, New version: 1.6.2]
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    `expected` is NULL
    
    Error in expression 26 of position.Rmd: plot(node_in_structural(to_named(ison_algebra), k = "elbow"))
    Backtrace:
        ▆
     1. ├─testthat::expect_null(...) at test-tutorials_netrics.R:10:5
     2. │ └─testthat::quasi_label(enquo(object), label)
     3. │   └─rlang::eval_bare(expr, quo_get_env(quo))
     4. └─migraph:::check_tute_functions(tute)
     5.   └─testthat::expect_null(...) at ./helper-functions.R:120:5
    
    [ FAIL 2 | WARN 0 | SKIP 3 | PASS 837 ]
    Error:
    ! Test failures.
    Execution halted

```
