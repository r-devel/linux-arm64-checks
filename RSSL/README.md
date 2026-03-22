# RSSL 0.9.8

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411751353

```
Package: RSSL
Check: whether package can be installed

AMD64: OK
  Used C compiler: ‘gcc (Ubuntu 13.3.0-6ubuntu2~24.04.1) 13.3.0’
  Used C++ compiler: ‘g++ (Ubuntu 13.3.0-6ubuntu2~24.04.1) 13.3.0’
ARM64: WARNING
  Found the following significant warnings:
    svm.cpp:42:38: warning: argument 1 range [18446744056529682432, 18446744073709551608] exceeds maximum object size 9223372036854775807 [-Walloc-size-larger-than=]
  See ‘/__w/linux-arm64-checks/linux-arm64-checks/RSSL.Rcheck/00install.out’ for details.
  Used C compiler: ‘gcc (Ubuntu 13.3.0-6ubuntu2~24.04.1) 13.3.0’
  Used C++ compiler: ‘g++ (Ubuntu 13.3.0-6ubuntu2~24.04.1) 13.3.0’
```
