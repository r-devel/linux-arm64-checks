# RcppAlgos 2.10.0

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411704984

```
Package: RcppAlgos
Check: S3 generic/method consistency

AMD64: OK
ARM64: WARNING
  sh: 1: /bin/kstat: not found
  See section ‘Generic functions and methods’ in the ‘Writing R
  Extensions’ manual.
Package: RcppAlgos
Check: for code/documentation mismatches

AMD64: OK
ARM64: WARNING
  sh: 1: /bin/kstat: not found
  sh: 1: /bin/kstat: not found
  sh: 1: /bin/kstat: not found
Package: RcppAlgos
Check: for missing documentation entries

AMD64: OK
ARM64: WARNING
  sh: 1: /bin/kstat: not found
  All user-level objects in a package should have documentation entries.
  See chapter ‘Writing R documentation files’ in the ‘Writing R
  Extensions’ manual.
Package: RcppAlgos
Check: replacement functions

AMD64: OK
ARM64: WARNING
  sh: 1: /bin/kstat: not found
  The argument of a replacement function which corresponds to the right
  hand side must be named ‘value’.
```
