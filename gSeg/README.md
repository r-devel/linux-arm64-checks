# gSeg 1.2

Latest run: 2026-11-14: https://github.com/r-devel/linux-arm64-checks/actions/runs/43588995444

```
Package: gSeg
Check: tests
AMD64: OK
    Running ‘canonical-defaults.R’
    Running ‘deep-regressions.R’
    Running ‘graph-robustness.R’
    Running ‘native-kernels.R’
    Running ‘numerical-stability.R’
    Running ‘second-review-regressions.R’
ARM64: ERROR
    Running ‘canonical-defaults.R’
    Running ‘deep-regressions.R’
    Running ‘graph-robustness.R’
    Running ‘native-kernels.R’
  Running the tests in ‘tests/native-kernels.R’ failed.
  Last 13 lines of output:
    > library(gSeg)
    > fd<-getFromNamespace(".gseg_fast_dist","gSeg");x5<-getFromNamespace(".gseg_native_x5","gSeg");x3<-getFromNamespace(".gseg_graph_x3","gSeg")
    > bits<-function(z)writeBin(as.double(z),raw(),size=8)
    > ncases<-0L
    > for(n in c(2:9,17,50))for(d in c(1,2,3,4,5,7,16,31,200))for(kind in c("random","integer","tiny","huge","offset","duplicate")){
    +  set.seed(53+n+d);x<-matrix(rnorm(n*d),n)
    +  if(kind=="integer")x<-round(x*3)
    +  if(kind=="tiny")x<-x*1e-160
    +  if(kind=="huge")x<-x*1e160
    +  if(kind=="offset")x<-1e150+x*1e140
    +  if(kind=="duplicate")x[2,]<-x[1,]
    +  stopifnot(identical(bits(stats::dist(x)),bits(fd(x))));ncases<-ncases+1L
    + }
    Error: identical(bits(stats::dist(x)), bits(fd(x))) is not TRUE
    Execution halted

```
