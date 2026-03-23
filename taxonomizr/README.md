# taxonomizr 0.11.1

Run: https://github.com/r-devel/linux-arm64-checks/actions/runs/23415142442

```
Package: taxonomizr
Check: examples

AMD64: OK
ARM64: ERROR
  Running examples in ‘taxonomizr-Ex.R’ failed
  The error most likely occurred in:
  
  > ### Name: accessionToTaxa
  > ### Title: Convert accessions to taxa
  > ### Aliases: accessionToTaxa
  > 
  > ### ** Examples
  > 
  > taxa<-c(
  +  "accession\taccession.version\ttaxid\tgi",
  +  "Z17427\tZ17427.1\t3702\t16569",
  +  "Z17428\tZ17428.1\t3702\t16570",
  +  "Z17429\tZ17429.1\t3702\t16571",
  +  "Z17430\tZ17430.1\t3702\t16572",
  +  "X62402\tX62402.1\t9606\t30394"
  + )
  > inFile<-tempfile()
  > sqlFile<-tempfile()
  > writeLines(taxa,inFile)
  > read.accession2taxid(inFile,sqlFile,vocal=FALSE)
  Error in trimTaxa(ii, tmp, 1:3) : 
    Could not write to file. Out of disk space?
  Calls: read.accession2taxid -> trimTaxa
  Execution halted
Package: taxonomizr
Check: tests

AMD64: OK
    Running ‘testthat.R’
ARM64: FAILURE
```
