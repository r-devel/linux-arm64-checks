# ARCokrig 0.1.3

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411223252

```
Package: ARCokrig
Check: examples

AMD64: OK
ARM64: ERROR
  Running examples in ‘ARCokrig-Ex.R’ failed
  The error most likely occurred in:
  
  > ### Name: ARCokrig
  > ### Title: Fit the AR-Cokriging model and make predictions
  > ### Aliases: ARCokrig
  > 
  > ### ** Examples
  > 
  > 
  > ##############################################################
  > ##############################################################
  > ############ Example
  > Funcc = function(x){
  +   return(0.5*(6*x-2)^2*sin(12*x-4)+10*(x-0.5)-5)
  + }
  > 
  > Funcf = function(x){
  +   z1 = Funcc(x)
  +   z2 = 2*z1-20*x+20 + sin(10*cos(5*x))
  +   return(z2)
  + }
  > 
  > #####################################################################
  > ###### Nested design 
  > #####################################################################
  > Dc <- seq(-1,1,0.1)
  > indDf <- c(1, 3, 6, 8, 10, 13, 17, 21)
  > zc <- Funcc(Dc)
  > Df <- Dc[indDf]
  > zf <- Funcf(Df)
  > 
  > input.new = as.matrix(seq(-1,1,length.out=200))
  > 
  > 
  > ## fit and predict with the AR-Cokriging model
  > 
  > out = ARCokrig(formula=list(~1,~1+x1), output=list(c(zc), c(zf)),
  +               input=list(as.matrix(Dc), as.matrix(Df)),
  +               cov.model="matern_5_2",
  +               input.new=input.new)
  [1] "optimization error, skip t=1"
  [1] "Error in chol.default(R) : the leading minor of order 2 is not positive\n"
  attr(,"class")
  [1] "try-error"
  attr(,"condition")
  <simpleError in chol.default(R): the leading minor of order 2 is not positive>
  [1] "optimization error, skip t=2"
  [1] "Error in chol.default(R) : the leading minor of order 2 is not positive\n"
  attr(,"class")
  [1] "try-error"
  attr(,"condition")
  <simpleError in chol.default(R): the leading minor of order 2 is not positive>
  Error in chol.default(R) : the leading minor of order 2 is not positive
  Calls: ARCokrig -> cokm.predict -> chol -> chol.default
  Execution halted
```
