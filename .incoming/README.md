## Incoming pipeline

The results from the [special/linux-arm64/](https://cran.r-project.org/incoming/special/linux-arm64/) dir in CRAN are stored under the `.incoming` directory. To get the results on your server, simply clone this repository (only do this once):

```sh
# Run this one time!
git clone https://github.com/r-devel/linux-arm64-checks
```

Each time you want to sync to the latest results, just run `./sync.sh` in this directory:

```sh
cd linux-arm64-checks
./sync.sh
```

So our `./sync.sh` script replaces the `rsync` command to update files; otherwise the steps are the same as the ssh pipelines. Old results are automatically deleted as well.
