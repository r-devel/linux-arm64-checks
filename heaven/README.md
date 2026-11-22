# heaven 2026.10.30

Latest run: 2026-11-22: https://github.com/r-devel/linux-arm64-checks/actions/runs/44966750036

```
Package: heaven
Check: examples
AMD64: OK
ARM64: ERROR
  Running examples in ‘heaven-Ex.R’ failed
  The error most likely occurred in:
  
  > ### Name: medicinMacro
  > ### Title: Medicin macro to estimate prescription lengths and averages
  > ### Aliases: medicinMacro
  > 
  > ### ** Examples
  > 
  > set.seed(05021992)
  > library(data.table)
  
  Attaching package: ‘data.table’
  
  The following object is masked from ‘package:base’:
  
      %notin%
  
  > N=20
  > packs = list("R03AK11"=list(c(750,75),c(500,200),c(400,200)),
  +              "R03AL03"=list(c(750,75),c(500,200),c(400,200)),
  +              "C01CA01"=list(c(200,100),c(750,30)))
  > lmdb=simPrescriptionData(N,packages=packs)
  > lpr=simAdmissionData(N)
  > lpr <- getAdmLimits(lpr,collapse=TRUE)
  No data errors.
  Nothing to collapse.
  > drug1 = list(atc=c("R03AK11","R03AL03","R03AC02","R03AC04","R03AC19",
  +                     "R03AL02","R03AA01","R03AC18","R03AL01"),
  +              maxdepot=4000,
  +              period=as.Date(c("1995-01-01", "2012-12-31")),
  +              prescriptionwindow=2,
  +              doses=list(value=c(750,500,400,200,75),
  +                         min = c(250,200,200,100,25),
  +                         max = c(1000,600,800,600,100),
  +                         def = c(750,500,400,200,75)))
  > drug2=list(atc=c("C01CA01","C01AA05"),
  +            maxdepot=4000,
  +            period=as.Date(c("1995-01-01", "2012-12-31")),
  +            prescriptionwindow=2,
  +            doses=list(value=c(200, 400, 500,750),
  +                       min = c(100, 200, 250,750),
  +                       max = c(300, 800, 1000,750),
  +                       def = c(200, 400, 500,750)))
  > x=medicinMacro(drugs=list("drug1"=drug1,"drug2"=drug2),drugdb=lmdb,admdb=lpr)
  > x$drug1
  Key: <pnr, firstday>
        pnr  dose   firstday    lastday exposure.days
      <num> <num>     <Date>     <Date>    <difftime>
   1:     1    75 1995-01-01 1995-05-18      137 days
   2:     1   100 1995-05-18 2008-06-15     4777 days
   3:     2    75 1995-01-01 1995-02-16       46 days
   4:     2   100 1995-02-16 2002-05-22     2652 days
   5:     3    75 1995-01-01 1995-01-22       21 days
   6:     3   100 1995-01-22 2003-02-24     2955 days
   7:     4    75 1995-01-01 1995-03-03       61 days
   8:     4   100 1995-03-03 2001-08-15     2357 days
   9:     5    75 1995-01-01 1995-01-10        9 days
  10:     5   100 1995-01-10 1996-03-08      423 days
  11:     5     0 1996-03-08 1996-03-24       16 days
  12:     5   100 1996-03-24 2001-02-12     1786 days
  13:     6    75 1995-01-01 1995-01-20       19 days
  14:     6   100 1995-01-20 2000-04-14     1911 days
  15:     7    75 1995-01-01 1995-03-18       76 days
  16:     7   100 1995-03-18 2002-09-13     2736 days
  17:     8    75 1995-01-01 1995-02-04       34 days
  18:     8   100 1995-02-04 2005-09-06     3867 days
  19:     9    75 1995-01-01 1995-01-21       20 days
  20:     9   100 1995-01-21 2004-02-05     3302 days
  21:    10    75 1995-01-01 1995-06-27      177 days
  22:    10   100 1995-06-27 2000-03-11     1719 days
  23:    11    75 1995-01-01 1995-01-05        4 days
  24:    11   100 1995-01-05 2004-02-12     3325 days
  25:    12    75 1995-01-01 1995-03-02       60 days
  26:    12   100 1995-03-02 2001-03-09     2199 days
  27:    13    75 1995-01-01 1995-02-06       36 days
  28:    13   100 1995-02-06 2000-05-28     1938 days
  29:    14    75 1995-02-26 1995-03-14       16 days
  30:    14   100 1995-03-14 1998-08-15     1250 days
  31:    14     0 1998-08-15 1998-10-23       69 days
  32:    14   100 1998-10-23 2001-04-24      914 days
  33:    15    75 1995-01-01 1995-02-26       56 days
  34:    15   100 1995-02-26 2001-12-19     2488 days
  35:    16    75 1995-01-01 1995-01-06        5 days
  36:    16   100 1995-01-06 2002-01-20     2571 days
  37:    17    75 1995-01-01 1995-03-28       86 days
  38:    17   100 1995-03-28 1995-12-22      269 days
  39:    17     0 1995-12-22 1996-03-04       73 days
  40:    17   100 1996-03-04 2006-04-02     3681 days
  41:    18    75 1995-01-01 1995-05-05      124 days
  42:    18   100 1995-05-05 2004-02-08     3201 days
  43:    19    75 1995-01-01 1995-01-09        8 days
  44:    19   100 1995-01-09 2008-04-15     4845 days
  45:    20    75 1995-01-01 1995-05-20      139 days
  46:    20   100 1995-05-20 2000-09-18     1948 days
        pnr  dose   firstday    lastday exposure.days
      <num> <num>     <Date>     <Date>    <difftime>
  > 
  > ## without admdata
  > x1=medicinMacro(drugs=list("drug1"=drug1,"drug2"=drug2),drugdb=lmdb,admdb=NULL)
  Error: Mat::elem(): index out of bounds
  Execution halted

```
