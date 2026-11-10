# sbm 0.4.7

Latest run: 2026-11-10: https://github.com/r-devel/linux-arm64-checks/actions/runs/42853599432

```
Package: sbm [Old version: 1.0.0, New version: 0.4.7]
Check: tests
AMD64: OK
    Running ‘spelling.R’
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘spelling.R’
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Actual comparison: 0.001074416746 >= 0.000000000001
    Difference: 0.001074416745 >= 0
    ── Failure ('test-SimpleSBM_fit_covariates.R:175:7'): SimpleSBM_fit 'Bernoulli' model, directed, one covariate ──
    Expected `rmse(pred_bm, pred_sbm)` < 1e-12.
    Actual comparison: 0.006415651445 >= 0.000000000001
    Difference: 0.006415651444 >= 0
    ── Failure ('test-SimpleSBM_fit_covariates.R:175:7'): SimpleSBM_fit 'Bernoulli' model, directed, one covariate ──
    Expected `rmse(pred_bm, pred_sbm)` < 1e-12.
    Actual comparison: 0.006906552831 >= 0.000000000001
    Difference: 0.006906552830 >= 0
    
    [ FAIL 12 | WARN 0 | SKIP 0 | PASS 1039 ]
    Error:
    ! Test failures.
    Execution halted

```
