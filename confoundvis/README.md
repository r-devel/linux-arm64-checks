# confoundvis 0.4.0

Latest run: 2026-11-23: https://github.com/r-devel/linux-arm64-checks/actions/runs/45145977421

```
Package: confoundvis
Check: examples
AMD64: OK
ARM64: ERROR
  Running examples in ‘confoundvis-Ex.R’ failed
  The error most likely occurred in:
  
  > ### Name: from_iv_sensemakr
  > ### Title: Convert an iv.sensemakr result to a confoundsens path
  > ### Aliases: from_iv_sensemakr
  > 
  > ### ** Examples
  > 
  > ## Don't show: 
  > if (requireNamespace("iv.sensemakr", quietly = TRUE)) withAutoprint({ # examplesIf
  + ## End(Don't show)
  + data("card", package = "iv.sensemakr")
  + xm <- model.matrix(~ exper + expersq + black + south + smsa + reg661 +
  +   reg662 + reg663 + reg664 + reg665 + reg666 + reg667 + reg668 + smsa66,
  +   data = card)
  + fit <- iv.sensemakr::iv_fit(card$lwage, card$educ, card$nearc4, xm)
  + s <- iv.sensemakr::sensemakr(fit, benchmark_covariates = c("black", "smsa"))
  + path <- from_iv_sensemakr(s)
  + robustness_points(path)
  + sens_report(path)
  + ## Don't show: 
  + }) # examplesIf
  > data("card", package = "iv.sensemakr")
  > xm <- model.matrix(~exper + expersq + black + south + smsa + reg661 + 
  +     reg662 + reg663 + reg664 + reg665 + reg666 + reg667 + reg668 + smsa66, data = card)
  > fit <- iv.sensemakr::iv_fit(card$lwage, card$educ, card$nearc4, xm)
  > s <- iv.sensemakr::sensemakr(fit, benchmark_covariates = c("black", "smsa"))
  > path <- from_iv_sensemakr(s)
  > robustness_points(path)
  Error in if (s0 == 0) s0 <- 1 : missing value where TRUE/FALSE needed
  Calls: withAutoprint ... withVisible -> eval -> eval -> robustness_points -> lapply -> FUN
  Execution halted

Package: confoundvis
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Backtrace:
        ▆
     1. ├─testthat::expect_match(...) at test-iv_sensemakr.R:60:3
     2. │ └─testthat::quasi_label(enquo(object), label)
     3. │   └─rlang::eval_bare(expr, quo_get_env(quo))
     4. ├─base::paste(sens_report(p)$text, collapse = " ")
     5. └─confoundvis::sens_report(p)
     6.   └─confoundvis::robustness_points(x, alpha = alpha)
     7.     └─base::lapply(...)
     8.       └─confoundvis (local) FUN(X[[i]], ...)
    
    [ FAIL 5 | WARN 2 | SKIP 0 | PASS 392 ]
    Error:
    ! Test failures.
    Execution halted

```
