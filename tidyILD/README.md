# tidyILD 0.4.0

Latest run: 2026-04-19: https://github.com/r-devel/linux-arm64-checks/actions/runs/24619072569

```
Package: tidyILD
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
      2. │ └─base::withCallingHandlers(...)
      3. └─tidyILD::ild_lme(...)
      4.   └─lme4::lmer(formula, data = data, ...)
      5.     └─lme4::optimizeLmer(...)
      6.       └─lme4:::optwrap(...)
      7.         ├─base::withCallingHandlers(...)
      8.         ├─base::do.call(optfun, arglist)
      9.         └─minqa (local) `<fn>`(...)
     10.           └─minqa (local) `<fn>`(`<dbl>`)
     11.             └─lme4 (local) fn(x, ...)
    
    [ FAIL 2 | WARN 141 | SKIP 20 | PASS 890 ]
    Error:
    ! Test failures.
    Execution halted

```
