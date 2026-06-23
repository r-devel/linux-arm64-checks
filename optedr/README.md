# optedr 3.0.0

Latest run: 2026-06-23: https://github.com/r-devel/linux-arm64-checks/actions/runs/28027069467

```
Package: optedr
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
      2. │ └─testthat:::expect_condition_matching_(...)
      3. │   └─testthat:::quasi_capture(...)
      4. │     ├─testthat (local) .capture(...)
      5. │     │ └─base::withCallingHandlers(...)
      6. │     └─rlang::eval_bare(quo_get_expr(.quo), quo_get_env(.quo))
      7. ├─base::suppressWarnings(...)
      8. │ └─base::withCallingHandlers(...)
      9. └─optedr::opt_des(...)
     10.   └─optedr:::WFMult(...)
     11.     └─optedr:::DWFMult(...)
    
    [ FAIL 1 | WARN 1 | SKIP 1 | PASS 417 ]
    Error:
    ! Test failures.
    Execution halted

```
