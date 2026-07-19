# gsDesign2 1.1.9

Latest run: 2026-07-19: https://github.com/r-devel/linux-arm64-checks/actions/runs/29669652320

```
Package: gsDesign2
Check: tests
AMD64: OK
    Running ‘test-all.R’
ARM64: ERROR
    Running ‘test-all.R’
  Running the tests in ‘tests/test-all.R’ failed.
  Last 13 lines of output:
    Testing testit/test-independent-wlr_weight.R... OK
    Testing testit/test-independent-as_gt.md... OK
    Testing testit/test-independent-as_rtf.md... OK
    Error: -- Assertion failed: Single analysis --
       x1$analysis$event (LHS) ==>
        num 280
       ----------
        num 280
       <== (RHS) u2$Events
       
       Detailed diff (- LHS, + RHS):
       - 279.72639477630287
       + 279.72639477630293
       x1$analysis$event %==% u2$Events is not TRUE but FALSE at testit/test-developer-gs_design_ahr.R#22
    Execution halted

```
