# Gtheory4LLM 1.0.0

Latest run: 2026-11-08: https://github.com/r-devel/linux-arm64-checks/actions/runs/42442836777

```
Package: Gtheory4LLM
Check: tests
AMD64: OK
    Running ‘package-analysis-report.R’
    Running ‘package-argument-parity.R’
    Running ‘package-batch-reliability.R’
    Running ‘package-batch.R’
    Running ‘package-binary-probabilities.R’
    Running ‘package-bootstrap.R’
    Running ‘package-categorical-target-moments.R’
    Running ‘package-categorical-target-numerics.R’
    Running ‘package-characterization.R’
    Running ‘package-dense-memory-guard.R’
    Running ‘package-development.R’
    Running ‘package-discrete-backend.R’
    Running ‘package-discrete-boundary-escape.R’
    Running ‘package-discrete-controls.R’
    Running ‘package-discrete-domain.R’
    Running ‘package-discrete-gradient-fit.R’
    Running ‘package-discrete-gradient-information.R’
    Running ‘package-discrete-gradient.R’
    Running ‘package-discrete-information.R’
    Running ‘package-discrete-safety.R’
    Running ‘package-discrete-scaling.R’
    Running ‘package-engines.R’
    Running ‘package-formula-interface.R’
    Running ‘package-fuzz-inputs.R’
    Running ‘package-gaussian-initialization.R’
    Running ‘package-gaussian-starts.R’
    Running ‘package-installed-examples.R’
    Running ‘package-laplace-check.R’
    Running ‘package-mixed-model.R’
    Running ‘package-native-workflow.R’
    Running ‘package-nested-designs.R’
    Running ‘package-nominal-reliability.R’
    Running ‘package-nominal-tails.R’
    Running ‘package-ordinal-tail.R’
    Running ‘package-outcome-profile.R’
    Running ‘package-planning.R’
    Running ‘package-preflight.R’
    Running ‘package-properties.R’
    Running ‘package-reporting.R’
    Running ‘package-response-third.R’
    Running ‘package-retry-behavior.R’
    Running ‘package-selected-inverse.R’
    Running ‘package-simulation.R’
    Running ‘package-smoke.R’
    Running ‘package-sparse-envelope.R’
    Running ‘package-sparse-estimated.R’
    Running ‘package-sparse-resources.R’
    Running ‘package-staged-diagnostics.R’
    Running ‘package-standard-methods.R’
    Running ‘package-stationarity-validity.R’
    Running ‘package-tuple-keys.R’
    Running ‘package-uncertainty.R’
    Running ‘package-user-interface.R’
    Running ‘package-visualizations.R’
ARM64: ERROR
    Running ‘package-analysis-report.R’
    Running ‘package-argument-parity.R’
    Running ‘package-batch-reliability.R’
    Running ‘package-batch.R’
    Running ‘package-binary-probabilities.R’
    Running ‘package-bootstrap.R’
    Running ‘package-categorical-target-moments.R’
    Running ‘package-categorical-target-numerics.R’
    Running ‘package-characterization.R’
    Running ‘package-dense-memory-guard.R’
    Running ‘package-development.R’
    Running ‘package-discrete-backend.R’
    Running ‘package-discrete-boundary-escape.R’
    Running ‘package-discrete-controls.R’
    Running ‘package-discrete-domain.R’
    Running ‘package-discrete-gradient-fit.R’
    Running ‘package-discrete-gradient-information.R’
    Running ‘package-discrete-gradient.R’
    Running ‘package-discrete-information.R’
    Running ‘package-discrete-safety.R’
    Running ‘package-discrete-scaling.R’
    Running ‘package-engines.R’
    Running ‘package-formula-interface.R’
    Running ‘package-fuzz-inputs.R’
    Running ‘package-gaussian-initialization.R’
    Running ‘package-gaussian-starts.R’
    Running ‘package-installed-examples.R’
    Running ‘package-laplace-check.R’
    Running ‘package-mixed-model.R’
    Running ‘package-native-workflow.R’
    Running ‘package-nested-designs.R’
    Running ‘package-nominal-reliability.R’
    Running ‘package-nominal-tails.R’
    Running ‘package-ordinal-tail.R’
    Running ‘package-outcome-profile.R’
    Running ‘package-planning.R’
    Running ‘package-preflight.R’
    Running ‘package-properties.R’
    Running ‘package-reporting.R’
    Running ‘package-response-third.R’
    Running ‘package-retry-behavior.R’
    Running ‘package-selected-inverse.R’
    Running ‘package-simulation.R’
    Running ‘package-smoke.R’
  Running the tests in ‘tests/package-smoke.R’ failed.
  Last 13 lines of output:
    +   n <- table(response)
    +   expected <- -2 * sum(n * log(n / sum(n)))
    +   stopifnot(fit$numerically_accepted, abs(fit$minus2loglik - expected) < 1e-6)
    + }
    > binary <- gt_fit(d, "binary", design, gt_family("binary", "logit"), control = fixed(1))
    > ordinal <- gt_fit(d, "ordinal", design, gt_family("ordinal"), control = fixed(1))
    Warning message:
    Discrete fit did not converge under numerical acceptance checks. Inspect gt_diagnostics(fit); coefficients and D studies are unavailable until the fit is numerically accepted. 
    > nominal <- gt_fit(d, "nominal", design, gt_family("categorical", reference = "blue"), control = fixed(2))
    > check_likelihood(binary, d$binary)
    > check_likelihood(ordinal, d$ordinal)
    Error in check_likelihood(ordinal, d$ordinal) : 
      fit$numerically_accepted is not TRUE
    Calls: check_likelihood -> stopifnot
    Execution halted

```
