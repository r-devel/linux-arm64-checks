# taxonomizr 0.11.1

Latest run: 2026-10-18: https://github.com/r-devel/linux-arm64-checks/actions/runs/39091198579

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
AMD64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
      1. ├─testthat::expect_error(...) at test_taxa.R:974:3
      2. │ └─testthat:::quasi_capture(...)
      3. │   ├─testthat (local) .capture(...)
      4. │   │ └─base::withCallingHandlers(...)
      5. │   └─rlang::eval_bare(quo_get_expr(.quo), quo_get_env(.quo))
      6. ├─taxonomizr:::resumableDownload("file://NOTAREALFILE.FAKE", tmpFile2)
      7. │ └─curl::multi_download(...)
      8. │   └─base::lapply(handles, handle_data)
      9. │     └─curl (local) FUN(X[[i]], ...)
     10. └─curl:::raise_libcurl_error(27L, "Out of memory")
    
    [ FAIL 1 | WARN 0 | SKIP 0 | PASS 378 ]
    Error:
    ! Test failures.
    Execution halted
ARM64: FAILURE

```
