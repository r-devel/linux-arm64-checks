# tidyILD 0.4.0

Latest run: 2026-05-24: https://github.com/r-devel/linux-arm64-checks/actions/runs/26350133911

```
Package: tidyILD
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    • regression_local_level not implemented in ild_kfas(); see
      inst/dev/KFAS_V1_BACKEND.md (1): 'test-kfas-extended.R:136:3'
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test-contract-regression.R:12:3'): contract: regular spacing + decomposed predictors — dense bundle, tidy/augment, plots, no guardrail methods ──
    Expected `grepl("Methodological cautions (tidyILD guardrails)", m, fixed = TRUE)` to be FALSE.
    Differences:
    `actual`:   TRUE 
    `expected`: FALSE
    
    
    [ FAIL 1 | WARN 142 | SKIP 20 | PASS 893 ]
    Error:
    ! Test failures.
    Execution halted

```
