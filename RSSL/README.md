# RSSL 0.9.8

Latest run: 2026-06-28: https://github.com/r-devel/linux-arm64-checks/actions/runs/28309134542

```
Package: RSSL
Check: whether package can be installed
AMD64: OK
  Used C compiler: ‘x86_64-linux-gnu-gcc (Ubuntu 15.2.0-16ubuntu1) 15.2.0’
  Used C++ compiler: ‘x86_64-linux-gnu-g++ (Ubuntu 15.2.0-16ubuntu1) 15.2.0’
ARM64: WARNING
  Found the following significant warnings:
    svm.cpp:42:38: warning: argument 1 range [18446744056529682432, 18446744073709551608] exceeds maximum object size 9223372036854775807 [-Walloc-size-larger-than=]
  See ‘/__w/linux-arm64-checks/linux-arm64-checks/RSSL.Rcheck/00install.out’ for details.
  Used C compiler: ‘aarch64-linux-gnu-gcc (Ubuntu 15.2.0-16ubuntu1) 15.2.0’
  Used C++ compiler: ‘aarch64-linux-gnu-g++ (Ubuntu 15.2.0-16ubuntu1) 15.2.0’

```
