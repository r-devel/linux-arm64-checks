# nprcgenekeepr 2.0.0

Latest run: 2026-08-16: https://github.com/r-devel/linux-arm64-checks/actions/runs/31918922750

```
Package: nprcgenekeepr
Check: tests
AMD64: OK
    Running ‘spelling.R’
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘spelling.R’
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Expected `res$rows` to equal 3L.
    Differences:
    1/1 mismatches
    [1] 0 - 3 == -3
    all 3 founder records survive the read + QC
    ── Failure ('test_modInput_incomplete_final_line.R:81:3'): read.table upload path muffles incomplete-final-line, keeps rows ──
    Expected `res$errors` to equal 0L.
    Differences:
    1/1 mismatches
    [1] 1 - 0 == 1
    
    [ FAIL 4 | WARN 0 | SKIP 231 | PASS 3096 ]
    Error:
    ! Test failures.
    Execution halted

```
