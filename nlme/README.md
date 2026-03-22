# nlme 3.1-168

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411598525

```
Package: nlme
Check: tests

AMD64: OK
    Processing ‘extras.Rin’
    Running ‘anova.gls.R’
    Running ‘augPred_lab.R’
    Running ‘augPredmissing.R’
    Running ‘coef.R’
    Comparing ‘coef.Rout’ to ‘coef.Rout.save’ ... OK
    Running ‘contrMat.R’
    Running ‘corMatrix.R’
    Running ‘corStruct.R’
    Running ‘data.frame.R’
    Running ‘deparse.R’
    Running ‘deviance.R’
    Running ‘fitted.R’
    Running ‘getData.R’
    Running ‘getVarCov.R’
    Running ‘gls.R’
    Running ‘gnls-ch8.R’
    Running ‘lme.R’
    Comparing ‘lme.Rout’ to ‘lme.Rout.save’ ... OK
    Running ‘lmList.R’
    Running ‘missing.R’
    Comparing ‘missing.Rout’ to ‘missing.Rout.save’ ... OK
    Running ‘nlme.R’
    Running ‘nlme2.R’
    Running ‘predict.lme.R’
    Running ‘scoping.R’
    Running ‘sigma-fixed-etc.R’
    Running ‘updateLme.R’
    Running ‘varConstProp.R’
    Running ‘varFixed.R’
    Running ‘varIdent.R’
ARM64: ERROR
    Processing ‘extras.Rin’
    Running ‘anova.gls.R’
    Running ‘augPred_lab.R’
    Running ‘augPredmissing.R’
    Running ‘coef.R’
    Comparing ‘coef.Rout’ to ‘coef.Rout.save’ ... OK
    Running ‘contrMat.R’
    Running ‘corMatrix.R’
    Running ‘corStruct.R’
    Running ‘data.frame.R’
    Running ‘deparse.R’
    Running ‘deviance.R’
    Running ‘fitted.R’
    Running ‘getData.R’
    Running ‘getVarCov.R’
    Running ‘gls.R’
  Running the tests in ‘tests/gls.R’ failed.
  Last 13 lines of output:
    > stopifnot(all.equal(
    +     predict(fm1, data.frame(Time = 71, Diet = c("2", "3"), stringsAsFactor = FALSE)),
    +     predict(fm1, data.frame(Time = 71, Diet = c("2", "3"), stringsAsFactor = TRUE))))
    > ## in nlme <= 3.1-155, using character input failed with
    > ## Error in X[, names(cf), drop = FALSE] : subscript out of bounds
    > tools::assertError(predict(fm1, data.frame(Time = 71, Diet = 2)), verbose = TRUE)
    Asserted error: contrasts apply only to factors
    > ## more helpful error + warning now
    > 
    > ## PR#17226: same for predict.gnls(), also without intercept
    > fm2 <- gnls(weight ~ f, data = BodyWeight, params = list(f ~ Diet - 1),
    +             start = rep(coef(fm1)[1], 3))
    Error in gnls(weight ~ f, data = BodyWeight, params = list(f ~ Diet -  : 
      step halving factor reduced below minimum in NLS step
    Execution halted
```
