# PFIM 8.0

Latest run: 2026-10-11: https://github.com/r-devel/linux-arm64-checks/actions/runs/38106997483

```
Package: PFIM
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    • src/init.c absent (installed tarball) (1): 'test-cpp-kernels.R:27:3'
    • tests_PFIM/resultats_de_references not found (1):
      'test-eval-opt-references.R:45:3'
    
    ══ Failed tests ════════════════════════════════════════════════════════════════
    ── Failure ('test-example-pk-mm.R:130:3'): Model PK 1cpt : MichaelisMenten1BolusSingleDose_VmKm ──
    Expected `detPopulationFim` to equal `valueDetPopulationFim`.
    Differences:
    actual != expected but don't know how to show the difference
    
    
    [ FAIL 1 | WARN 0 | SKIP 49 | PASS 1075 ]
    Error:
    ! Test failures.
    Execution halted

```
