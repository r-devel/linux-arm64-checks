# cmpp 0.0.2

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411277206

```
Package: cmpp
Check: examples

AMD64: OK
ARM64: ERROR
  Running examples in ‘cmpp-Ex.R’ failed
  The error most likely occurred in:
  
  > ### Name: CIF_Figs
  > ### Title: Plot Cumulative Incidence Functions (CIF) with Confidence
  > ###   Intervals
  > ### Aliases: CIF_Figs
  > 
  > ### ** Examples
  > 
  > library(cmpp)
  > data("fertility_data")
  > Nam <- names(fertility_data)
  > fertility_data$Education
    [1] 2 2 2 1 2 2 2 2 2 2 1 1 2 2 2 2 1 3 3 2 2 2 2 2 2 2 2 2 1 2 1 2 2 2 2 2 2
   [38] 2 1 2 3 2 2 1 2 2 2 2 2 2 2 1 2 2 2 1 2 2 2 2 2 1 1 2 2 3 3 2 2 2 2 2 2 3
   [75] 2 2 2 2 2 2 2 2 2 3 2 2 2 2 2 1 2 2 2 3 2 1 1 2 2 1 1 3 2 2 2 2 1 3 2 2 3
  [112] 3 2 2 2 2 2 2 2 2 3 2 2 2 2 2 3 2 2 2 2 2 2 2 2 2 3 2 2 2 2 2 3 2 2 2 2 3
  [149] 3 2 2 1 3 1 3 2 2 3 2 3 3 3 2 2 2 1 2 2 3 1 2 2 1 2 2 3 2 1 2 1 2 1 2 2 2
  [186] 2 1 2 2 2 1 3 2 2 2 2 3 1 2 2 2 2 2 2 2 2 3 2 1 3 1 3 2 2 2 2 3 2 3 2 2 2
  [223] 3 2 2 2 2 2 2 2 2 2 2 2 2 2 3 2 2 2 3 2 2 2 3 2 3 2 2 1 2 1 3 2 2 2 2 2 2
  [260] 2 3 1 2 2 2 2 2 2 2 2 2 2 2 3 2 2 2 2 2 1 1 2 1 2 2 2 2 2 1 2 2 2 2 2 2 1
  [297] 1 1 2 2 2 2 2 2 2 2 1 2 1 2 2 2 1 2 2 2 2 2 2 2 2 1 2 1 1 2 1 2 2 2 2 2 1
  [334] 2 3 2 3 3 2 3 2 3 2 2 3 2 2 3 2 2 1 3 2 3 2 2 3 3 3 3 2 2 2 1 3 2 2 2 2 2
  [371] 2 1 2 1 1 1 1 2 2 1 1 2 2 1 1 3 2 1 1 2 1 2 1 2 2 2 1 2 1 2 2 2 1 2 1 3 2
  [408] 2 2 3 2 1 2 1 3 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2
  [445] 1 2 2 2 2 2 1 3 1 2 3 3 2 1 2 2 2 1 2 2 2 3 2 2 2 2 3 2 2 2 2 2 2 3 3 2 1
  [482] 1 2 2 2 2 2 2 2 2 3 2 2 2 2 2 2 2 3 2 2 2 2 2 2 3 2 3 3 2 2 2 2 3 2 2 2 2
  [519] 3 1 2 2 3 2 2 2 2 3 2 2 2 3 2 3 2 1 1 2 3 2 3 3 2 2 2 2 3 2 3 2 2 2 3 3 2
  [556] 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 3 3 2 2 2 2 2 1 2 3 2 2 2 1 2 2 2 1 2 2 2 2
  [593] 2 2 2 2 2 2 2 1 2 2 2 2 2 2 2 2 2 3 2 2 2 3 2 2 1 2 2 1 2 1 2 2 2 1 2 1 1
  [630] 2 2 2 2 2 2 2 2 3 3 2 1 2 2 1 2 2 2 2 2 1 2 2
  attr(,"label")
  [1] Education Levels
  attr(,"labels")
         Illiterate Primary/Secondary  Higher Education 
                  1                 2                 3 
  Levels: 1 2 3
  > datt <- make_Dummy(fertility_data, features = c("Education"))
  > datt <- datt$New_Data 
  > datt['Primary_Secondary'] <- datt$`Education:2`
  > datt['Higher_Education'] <- datt$`Education:3`
  > datt$`Education:2` <- datt$`Education:3` <- NULL
  > datt2 <- make_Dummy(datt, features = 'Event')$New_Data
  > d1 <- datt2$`Event:2`
  > d2 <- datt2$`Event:3`
  > feat <- datt2[c('age', 'Primary_Secondary', 'Higher_Education')] |> 
  +    data.matrix()
  > timee <- datt2[['time']]
  > Initialize(feat, timee, d1, d2, 1e-10)
  > initial_params <- c(0.001, 0.001, 0.001, 0.001)
  > result <- CIF_res1(initial_params)
  Error in solve.default(Information_matrix[3:4, 3:4]) : 
    Lapack routine dgesv: system is exactly singular: U[2,2] = 0
  Calls: CIF_res1 -> solve -> solve.default
  Execution halted
```
