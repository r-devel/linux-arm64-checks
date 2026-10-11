# iSTATS 1.8

Latest run: 2026-10-11: https://github.com/r-devel/linux-arm64-checks/actions/runs/38107771062

```
Package: iSTATS
Check: tests
AMD64: OK
    Running ‘alignment-regions.R’
    Running ‘app-helpers.R’
    Running ‘app-ui-navigation.R’
    Running ‘icoshift-regression.R’
    Running ‘selected-regions.R’
    Running ‘session-isolation.R’
    Running ‘shiny-alignment.R’
    Running ‘shiny-flow.R’
    Running ‘shiny-selected-regions.R’
    Running ‘shiny-stocsy.R’
    Running ‘spectra-plot.R’
ARM64: ERROR
    Running ‘alignment-regions.R’
    Running ‘app-helpers.R’
  Running the tests in ‘tests/app-helpers.R’ failed.
  Last 13 lines of output:
    + }
    > y <- matrix(rnorm(52 * 8), 52, dimnames = list(NULL, paste0("c", 1:8)))
    > y[1, 1] <- NA; y[2, 2] <- Inf; y[, 3] <- NaN; y[1:50, 4] <- NA
    > shapiro_cases[[length(shapiro_cases) + 1L]] <- y
    > default_blocks <- helpers$.column_blocks
    > for (block_size in c(8192L, 3L)) {     # one block, and many uneven blocks
    +   helpers$.column_blocks <- function(columns, size = block_size)
    +     default_blocks(columns, size)
    +   for (m in c(cases, shapiro_cases)) {
    +     stopifnot(identical(helpers$.shapiro_p_values(m), reference_p(m)),
    +               identical(helpers$.spearman_ranks(m), reference_ranks(m)))
    +   }
    + }
    Error: identical(helpers$.shapiro_p_values(m), reference_p(m)) is not TRUE
    Execution halted

```
