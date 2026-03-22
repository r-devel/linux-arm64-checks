# hibayes 3.1.0

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23411442719

```
Package: hibayes
Check: examples

AMD64: OK
ARM64: ERROR
  Running examples in ‘hibayes-Ex.R’ failed
  The error most likely occurred in:
  
  > ### Name: ssbrm
  > ### Title: Single-step Bayes model
  > ### Aliases: ssbrm
  > 
  > ### ** Examples
  > 
  > # Load the example data attached in the package
  > pheno_file_path = system.file("extdata", "demo.phe", package = "hibayes")
  > pheno = read.table(pheno_file_path, header=TRUE)
  > 
  > bfile_path = system.file("extdata", "demo", package = "hibayes")
  > bin = read_plink(bfile_path, threads=1)
  Warning: Missing values in genotype exist!
  Imputing missing values by major genotype...
  > fam = bin$fam
  > geno = bin$geno
  > map = bin$map
  > 
  > pedigree_file_path = system.file("extdata", "demo.ped", package = "hibayes")
  > ped = read.table(pedigree_file_path, header=TRUE)
  > 
  > # For GS/GP
  > ## no environmental effects:
  > fit = ssbrm(T1~1, data=pheno, M=geno, M.id=fam[,2], pedigree=ped,
  + 	method="BayesCpi", niter=1000, nburn=600, thin=5, printfreq=100, threads=1)
  Error in if (sum(p < maf)) { : argument is not interpretable as logical
  Calls: ssbrm
  Execution halted
```
