# kamila 0.2.0

Latest run: 2026-09-20: https://github.com/r-devel/linux-arm64-checks/actions/runs/35493462477

```
Package: kamila
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
      old[1, ] 1.0000000 1.0000000 1.0000000 1.0000000  1.0
    - old[2, ] 0.4666667 0.4285714 0.5384615 0.8181818  0.2
    + new[2, ] 0.5909091 0.4285714 0.5384615 0.8181818  0.2
    
    
    ── Snapshots ───────────────────────────────────────────────────────────────────
    To review and process snapshots locally:
    * Locate check directory.
    * Copy 'tests/testthat/_snaps' to local package.
    * Run `testthat::snapshot_accept()` to accept all changes.
    * Run `testthat::snapshot_review()` to review all changes.
    [ FAIL 4 | WARN 1 | SKIP 0 | PASS 322 ]
    Error:
    ! Test failures.
    Execution halted

```
