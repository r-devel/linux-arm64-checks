# grates 1.8.1

Latest run: 2026-11-11: https://github.com/r-devel/linux-arm64-checks/actions/runs/43010609029

```
Package: grates
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    Differences:
    `actual[17:20]`:   "2017-W01" "2018-W01" "2019-W01" "1970-W01"
    `expected[17:20]`: "2017-W01" "2018-W01" "2019-W01" NA        
    
    ── Failure ('test-yearweek.R:66:5'): yearweek, january 1 dates ─────────────────
    Expected `as.character(dates_epi)` to be identical to `expected`.
    Differences:
    `actual[17:20]`:   "2017-W01" "2018-W01" "2019-W01" "1970-W01"
    `expected[17:20]`: "2017-W01" "2018-W01" "2019-W01" NA        
    
    
    [ FAIL 8 | WARN 0 | SKIP 12 | PASS 860 ]
    Error:
    ! Test failures.
    Execution halted

```
