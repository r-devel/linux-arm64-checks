# elmNNRcpp 1.0.5

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411332594

```
Package: elmNNRcpp
Check: tests

AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Time to complete : 0.0003387928 secs 
    [ FAIL 1 | WARN 0 | SKIP 0 | PASS 29 ]
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Error ('test-elm.R:5:3'): elm regression works ──────────────────────────────
    Error in `elm_train_rcpp(x, y, nhid, actfun, init_weights, bias, moorep_pseudoinv_tol, leaky_relu_alpha, seed, verbose)`: BLAS/LAPACK routine 'DLASCL' gave error code -4
    Backtrace:
        ▆
     1. └─elmNNRcpp::elm_train(xtr, ytr, nhid = 100, actfun = "sig") at test-elm.R:5:3
     2.   └─elmNNRcpp:::elm_train_rcpp(...)
    
    [ FAIL 1 | WARN 0 | SKIP 0 | PASS 29 ]
    Error:
    ! Test failures.
    Execution halted
```
