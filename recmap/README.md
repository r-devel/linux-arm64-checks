# recmap 1.0.20

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411718056

```
Package: recmap
Check: examples

AMD64: OK
ARM64: ERROR
  Running examples in ‘recmap-Ex.R’ failed
  The error most likely occurred in:
  
  > ### Name: recmapGA
  > ### Title: Genetic Algorithm Wrapper Function for recmap
  > ### Aliases: recmapGA
  > 
  > ### ** Examples
  > 
  > ## The default fitness function is currently defined as
  > function(idxOrder, Map, ...){
  + 
  +   Cartogram <- recmap(Map[idxOrder, ])
  +   # a map region could not be placed; 
  +   # accept only feasible solutions!
  +   
  +   if (sum(Cartogram$topology.error == 100) > 0){ return (0) }
  +   
  +   1 / sum(Cartogram$relpos.error)
  + }
  function (idxOrder, Map, ...) 
  {
      Cartogram <- recmap(Map[idxOrder, ])
      if (sum(Cartogram$topology.error == 100) > 0) {
          return(0)
      }
      1/sum(Cartogram$relpos.error)
  }
  > 
  > 
  > ## use Genetic Algorithms (GA >=3.0.0) as metaheuristic
  > set.seed(1)
  > 
  > ## https://github.com/luca-scr/GA/issues/52
  > if (Sys.info()['machine'] == "arm64") GA::gaControl(useRcpp = FALSE)
  > res <- recmapGA(V = checkerboard(4), pmutation = 0.25)
  Warning in recmap(Map[idxOrder, ]) :
    d4 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    d4 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    a3 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    d4 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    d4 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    a1 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    a1 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    a1 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    b4 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    a1 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    a1 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    b4 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    a1 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    d4 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    a1 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    b4 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    c1 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    b4 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    d4 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    a1 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    a1 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    a1 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    c1 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    a1 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    d4 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    a1 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    d4 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    a1 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    a1 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    d4 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    a1 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    a1 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    a1 could not be placed on the first attempt;
  Warning in recmap(Map[idxOrder, ]) :
    d4 could not be placed on the first attempt;
  Error: index error
  Execution halted
Package: recmap
Check: tests

AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
    <Rcpp::exception/C++Error/error/condition>
    Error: index error
    Backtrace:
        ▆
     1. └─base::lapply(...) at test-jss2711.R:10:3
     2.   └─recmap (local) FUN(X[[i]], ...)
     3.     └─recmap::recmapGA(V = checkerboard(4), pmutation = 0.25, parallel = FALSE) at test-jss2711.R:14:5
     4.       └─GA::ga(...)
     5.         └─GA (local) crossover(object, parents)
     6.           └─GA:::gaperm_oxCrossover_Rcpp(object, parents)
    
    [ FAIL 1 | WARN 93 | SKIP 1 | PASS 23 ]
    Error:
    ! Test failures.
    Execution halted
```
