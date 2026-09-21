# rqti 1.3.0

Latest run: 2026-09-21: https://github.com/r-devel/linux-arm64-checks/actions/runs/35644250701

```
Package: rqti
Check: examples
AMD64: OK
ARM64: ERROR
  Running examples in ‘rqti-Ex.R’ failed
  The error most likely occurred in:
  
  > ### Name: section
  > ### Title: Create a section as part of a test content
  > ### Aliases: section
  > 
  > ### ** Examples
  > 
  > sc <- new("SingleChoice", prompt = "Question", choices = c("A", "B", "C"))
  > es <- new("Essay", prompt = "Question")
  > # Since ready-made S4 "AssessmentItem" objects are taken, in this example a
  > #permanent section consisting of two tasks is created.
  > s <- section(c(sc, es), title = "Section with nonrandomized tasks")
  > 
  > # Since Rmd files with randomization of internal variables are taken,
  > #in this example 2 variants are created with a different seed number for each.
  > path <- system.file("rmarkdown/templates/", package='rqti')
  > file1 <- file.path(path, "singlechoice-simple/skeleton/skeleton.Rmd")
  > file2 <- file.path(path, "singlechoice-complex/skeleton/skeleton.Rmd")
  > s <- section(c(file1, file2), n_variants = 2,
  + title = "Section with two variants of tasks")
  Unknown option --syntax-highlighting.
  Try pandoc --help for more information.
  Error: pandoc document conversion failed with error 6
  Execution halted

Package: rqti
Check: tests
AMD64: OK
    Running ‘testthat.R’
ARM64: ERROR
    Running ‘testthat.R’
  Running the tests in ‘tests/testthat.R’ failed.
  Last 13 lines of output:
     3.     └─rmarkdown::pandoc_convert(input_file, options = options, wd = dir_name)
     4.       └─rmarkdown:::stop2(...)
    ── Error ('test-verify_qti.R:249:5'): verify_qti prints AssessmentTest validation summaries ──
    Error: pandoc document conversion failed with error 6
    Backtrace:
        ▆
     1. └─rqti::create_question_object(rmd_file) at test-verify_qti.R:249:5
     2.   └─rqti:::pandoc_html_convert(file_p, "_temp_pandoc.html", tdir)
     3.     └─rmarkdown::pandoc_convert(input_file, options = options, wd = dir_name)
     4.       └─rmarkdown:::stop2(...)
    
    [ FAIL 58 | WARN 0 | SKIP 20 | PASS 477 ]
    Error:
    ! Test failures.
    Execution halted

```
