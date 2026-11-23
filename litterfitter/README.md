# litterfitter 0.3.0

Latest run: 2026-11-23: https://github.com/r-devel/linux-arm64-checks/actions/runs/45105241018

```
Package: litterfitter
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
      `actual`: 0.0 52.0 0.0 0.0
    `expected`: 0.0  0.0 0.0 0.0
    
    cont.quality
    
    [ FAIL 2 | WARN 1 | SKIP 2 | PASS 932 ]
    Deleting unused snapshots: 'autoplot/autoplot-bootstrap.svg',
    'autoplot/autoplot-elementfit.svg', 'autoplot/autoplot-litfit-band.svg',
    'autoplot/autoplot-litfit-list.svg', 'autoplot/autoplot-litfit.svg',
    'plots/plot-bootstrap-all.svg', 'plots/plot-elementfit.svg',
    'plots/plot-litfit-band.svg', 'plots/plot-litfit-list.svg', and
    'plots/plot-litfit.svg'
    Error:
    ! Test failures.
    Execution halted

```
