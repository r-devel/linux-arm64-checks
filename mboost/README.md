# mboost 2.9-12

Latest run: 2026-07-15: https://github.com/r-devel/linux-arm64-checks/actions/runs/29421525048

```
Package: mboost
Check: tests
AMD64: NOTE
    Running ‘birds_Biometrics.R’
    Comparing ‘birds_Biometrics.Rout’ to ‘birds_Biometrics.Rout.save’ ... OK
    Running ‘bugfixes.R’
    Comparing ‘bugfixes.Rout’ to ‘bugfixes.Rout.save’ ... OK
    Running ‘regtest-baselearner.R’
    Comparing ‘regtest-baselearner.Rout’ to ‘regtest-baselearner.Rout.save’ ...
  12,19c12,20
  <     %+%, %O%, %X%, AdaExp, as.data.frame.varimp, AUC, bbs, Binomial,
  <     bkernel, blackboost, bmono, bmrf, bns, bols, boost_control, brad,
  <     brandom, bspatial, bss, btree, buser, Cindex, confint.glmboost,
  <     confint.mboost, CoxPH, cv, cvrisk, downstream.test, ExpectReg,
  <     extract, Family, fitted.mboost, FP, gamboost, GammaReg, GaussClass,
  <     Gaussian, GaussReg, Gehan, glmboost, Huber, Hurdle, IPCweights,
  <     Laplace, lines.mboost, lines.mboost.ci, Loglog, Lognormal, mboost,
  <     mboost_fit, mboost_intern, mstop, mstop<-, Multinomial, NBinomial,
  ---
  >     %+%, %O%, %X%, AUC, AdaExp, Binomial, Cindex, CoxPH, ExpectReg, FP,
  >     Family, GammaReg, GaussClass, GaussReg, Gaussian, Gehan, Huber,
  >     Hurdle, IPCweights, Laplace, Loglog, Lognormal, Multinomial,
  >     NBinomial, Poisson, PropOdds, QuantReg, RCG, Weibull,
  >     as.data.frame.varimp, bbs, bkernel, blackboost, bmono, bmrf, bns,
  >     bols, boost_control, brad, brandom, bspatial, bss, btree, buser,
  >     confint.glmboost, confint.mboost, cv, cvrisk, downstream.test,
  >     extract, fitted.mboost, gamboost, glmboost, lines.mboost,
  >     lines.mboost.ci, mboost, mboost_fit, mboost_intern, mstop, mstop<-,
  21,23c22,24
  <     plot.varimp, Poisson, predict.glmboost, predict.mboost,
  <     print.glmboost.ci, PropOdds, QuantReg, RCG, risk, selected.mboost,
  <     stabsel_parameters.mboost, stabsel.mboost, survFit, varimp, Weibull
  ---
  >     plot.varimp, predict.glmboost, predict.mboost, print.glmboost.ci,
  >     risk, selected.mboost, stabsel.mboost, stabsel_parameters.mboost,
  >     survFit, varimp
    Running ‘regtest-blackboost.R’
    Comparing ‘regtest-blackboost.Rout’ to ‘regtest-blackboost.Rout.save’ ... OK
    Running ‘regtest-family.R’
    Comparing ‘regtest-family.Rout’ to ‘regtest-family.Rout.save’ ... OK
    Running ‘regtest-gamboost.R’
    Comparing ‘regtest-gamboost.Rout’ to ‘regtest-gamboost.Rout.save’ ... OK
    Running ‘regtest-glmboost.R’
    Comparing ‘regtest-glmboost.Rout’ to ‘regtest-glmboost.Rout.save’ ... OK
    Running ‘regtest-hatmatrix.R’
    Comparing ‘regtest-hatmatrix.Rout’ to ‘regtest-hatmatrix.Rout.save’ ... OK
    Running ‘regtest-varimp.R’
    Comparing ‘regtest-varimp.Rout’ to ‘regtest-varimp.Rout.save’ ... OK
ARM64: ERROR
    Running ‘birds_Biometrics.R’
    Comparing ‘birds_Biometrics.Rout’ to ‘birds_Biometrics.Rout.save’ ... OK
    Running ‘bugfixes.R’
    Comparing ‘bugfixes.Rout’ to ‘bugfixes.Rout.save’ ... OK
    Running ‘regtest-baselearner.R’
  Running the tests in ‘tests/regtest-baselearner.R’ failed.
  Last 13 lines of output:
    > y <- rnorm(n)
    > ndf <- data.frame(x1 = x1[1:10], x2 = x2[1:10], f = f[1:10])
    > 
    > ### spatial
    > m1 <- gamboost(y ~ bbs(x1) %X% bbs(x2))
    Warning message:
    In .qr.rank.def.warn(r) :
      matrix is structurally rank deficient; using augmented matrix with additional 203 row(s) of zeros
    > m2 <- gamboost(y ~ bspatial(x1, x2, df = 16))
    Warning message:
    In .qr.rank.def.warn(r) :
      matrix is structurally rank deficient; using augmented matrix with additional 203 row(s) of zeros
    > stopifnot(max(abs(predict(m1) - predict(m2))) < sqrt(.Machine$double.eps))
    Error: max(abs(predict(m1) - predict(m2))) < sqrt(.Machine$double.eps) is not TRUE
    Execution halted

```
