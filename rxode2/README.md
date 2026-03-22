# rxode2 5.0.2

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411758515

```
Package: rxode2
Check: examples

AMD64: OK
ARM64: ERROR
  Running examples in ‘rxode2-Ex.R’ failed
  The error most likely occurred in:
  
  > ### Name: dfWishart
  > ### Title: This uses simulations to match the rse
  > ### Aliases: dfWishart
  > 
  > ### ** Examples
  > 
  > 
  > dfWishart(lotri::lotri(a+b~c(1, 0.5, 1)), 100)
  
   *** caught segfault ***
  address 0xfff07f8c5b54, cause 'invalid permissions'
  
  Traceback:
   1: withCallingHandlers(expr, warning = function(w) if (inherits(w,     classes)) tryInvokeRestart("muffleWarning"))
   2: suppressWarnings(.Call(`_rxode2_setGlobalSeed`, seed$seed))
   3: .rxSetSeed(.newSeed)
   4: rxWithSeed(seed, {    stats::uniroot(dfWishartCalcRse, lower = .lower, upper = .upper,         omega = omega, totN = totN, rse = rse, diag = diag)})
   5: dfWishart(lotri::lotri(a + b ~ c(1, 0.5, 1)), 100)
  An irrecoverable exception occurred. R is aborting now ...
  Segmentation fault (core dumped)
Package: rxode2
Check: tests

AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    27: test_code(code = exprs, env = env, reporter = get_reporter() %||%     StopReporter$new())
    28: source_file(path, env = env(env), desc = desc, shuffle = shuffle,     error_call = error_call)
    29: FUN(X[[i]], ...)
    30: lapply(test_paths, test_one_file, env = env, desc = desc, shuffle = shuffle,     error_call = error_call)
    31: doTryCatch(return(expr), name, parentenv, handler)
    32: tryCatchOne(expr, names, parentenv, handlers[[1L]])
    33: tryCatchList(expr, classes, parentenv, handlers)
    34: tryCatch(code, testthat_abort_reporter = function(cnd) {    cat(conditionMessage(cnd), "\n")    NULL})
    35: with_reporter(reporters$multi, lapply(test_paths, test_one_file,     env = env, desc = desc, shuffle = shuffle, error_call = error_call))
    36: test_files_serial(test_dir = test_dir, test_package = test_package,     test_paths = test_paths, load_helpers = load_helpers, reporter = reporter,     env = env, stop_on_failure = stop_on_failure, stop_on_warning = stop_on_warning,     desc = desc, load_package = load_package, shuffle = shuffle,     error_call = error_call)
    37: test_files(test_dir = path, test_paths = test_paths, test_package = package,     reporter = reporter, load_helpers = load_helpers, env = env,     stop_on_failure = stop_on_failure, stop_on_warning = stop_on_warning,     load_package = load_package, parallel = parallel, shuffle = shuffle)
    38: test_dir("testthat", package = package, reporter = reporter,     ..., load_package = "installed")
    39: test_check("rxode2")
    An irrecoverable exception occurred. R is aborting now ...
    Segmentation fault (core dumped)
```
