# Linux ARM64 checks

A cran "special check" to identify packages with problems specifically on arm64 linux.

## How it works

We check CRAN packages on both amd64 and arm64 runners using exactly the same setup. We flag packages that show a `WARNING` or `ERROR` on arm64 but not on amd64.

The checks run in the [rcheckserver](https://github.com/r-devel/rcheckserver) container which has the same system libraries as CRAN Debian servers.

## Feedback

This is a community project and also serves as a template to use GitHub actions for running custom CRAN special checks. For problems or suggestions please open an issue in this repository (no need to email CRAN).
