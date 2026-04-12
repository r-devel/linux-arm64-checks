# CompositionalSR 1.3

Latest run: 2026-04-12: https://github.com/r-devel/linux-arm64-checks/actions/runs/24296179489

```
Package: CompositionalSR
Check: examples
AMD64: OK
ARM64: ERROR
  Running examples in ‘CompositionalSR-Ex.R’ failed
  The error most likely occurred in:
  
  > ### Name: ICE plot for the alpha-ESF model
  > ### Title: ICE plot for the alpha-ESF model
  > ### Aliases: ice.aesf
  > 
  > ### ** Examples
  > 
  > data(fadn)
  > coords <- fadn[, 1:2]
  > y <- fadn[, 3:7]
  > x <- fadn[, 8, drop = FALSE]
  > mod <- alfa.esf(y, x, a = 0.1, coords = coords)
   25 spatial eigen-pairs
  > ice <- ice.aesf(mod$be, mod$gama, x, mod$X.esf, ind = 1)
  Error in plot.window(...) : need finite 'ylim' values
  Calls: ice.aesf ... <Anonymous> -> plot -> plot.default -> localWindow -> plot.window
  Execution halted

```
