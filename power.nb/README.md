# power.nb 0.1.0

Latest run: 2026-06-28: https://github.com/r-devel/linux-arm64-checks/actions/runs/28309523387

```
Package: power.nb
Check: examples
AMD64: OK
ARM64: ERROR
  Running examples in ‘power.nb-Ex.R’ failed
  The error most likely occurred in:
  
  > ### Name: power_fun_ss
  > ### Title: Fit a smooth power model for sample size estimation
  > ### Aliases: power_fun_ss
  > 
  > ### ** Examples
  > 
  > #' @examples
  > 
  > # Example structure only
  > set.seed(101)
  > n = 70
  > pval_est_list = list(rnorm(n),rnorm(n))
  > logmean_list = list(rnorm(n),rnorm(n))
  > logfoldchange_list = list(rnorm(n),rnorm(n))
  > nsample_vec <- c(20, 40)
  > out <- power_fun_ss(
  + pval_est_list = pval_est_list,
  + logmean_list = logmean_list,
  + nsample_vec = nsample_vec,
  + logfoldchange_list = logfoldchange_list,
  + alpha_level = 0.1
  + )
  Error: The simpler SCAM model failed to converge.
  Original error: inner loop 3; can't correct step size
  Execution halted

```
