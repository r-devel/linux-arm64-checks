# blocking 1.0.3

Latest run: 2026-07-12: https://github.com/r-devel/linux-arm64-checks/actions/runs/29176230169

```
Package: blocking
Check: tests
AMD64: OK
    Running ‘tinytest.R’
ARM64: ERROR
    Running ‘tinytest.R’
  Running the tests in ‘tests/tinytest.R’ failed.
  Last 13 lines of output:
     call| expect_equal(blocking(x = mat_x, y = mat_y, ann = "hnsw", control_ann = controls_ann(hnsw = list(M = 5, 
     call| -->    ef_s = 10, ef_c = 10))), structure(list(result = structure(list(x = c(1, 
     call| -->    1, 1, 1, 2, 2, 2, 2), y = c(5, 6, 7, 8, 1, 2, 3, 4), block = c(2, 
     call| -->    2, 2, 2, 1, 1, 1, 1), dist = c(1.19209289550781e-07, 0.0425729155540466, 
     call| -->    1.19209289550781e-07, 0.278312206268311, 0.0513166785240173, 
     call| -->    -1.19209289550781e-07, 0.0513166785240173, 0.225403368473053)), 
     call| -->    row.names = c(NA, -8), class = c("data.table", "data.frame")), 
     call| -->    method = "hnsw", deduplication = FALSE, representation = "custom_matrix", 
     call| -->    metrics = NULL, confusion = NULL, colnames = c("al", "an", 
     call| -->        "ho", "ij", "ja", "ki", "ko", "ls", "mo", "nt", "ow", 
     call| -->        "py", "sk", "ty", "wa", "yp", "yt", "on", "th"), graph = NULL), 
     call| -->    class = "blocking", n_x = 3, n_y = 8))
     diff| Component "result": Column 'dist': Mean relative difference: 1.837035e-07
    Error: 2 out of 95 tests failed
    Execution halted

```
