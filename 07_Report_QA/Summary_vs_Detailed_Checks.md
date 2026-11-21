# Summary Versus Detailed Checks

| Test ID | Objective | Recorded expectation | QA notes | Included PDF | Status |
| --- | --- | --- | --- | --- | --- |
| REP-02 | Confirm summary status agrees with detailed checks | Summary should not report PASS if fatigue/deflection checks fail | Notes record summary PASS while fatigue and total-load deflection were FAIL | PDF executive summary on physical page 3 says “Overall Design Status Fail”; detailed outputs also include failures | FAIL in QA notes; exact artifact/run mapping NEEDS INVESTIGATION |

## Discrepancy handling

The recorded finding must remain visible, but this PDF copy does not itself show an overall PASS in the extracted executive summary. The notes may refer to a different summary surface, report version, or run. Do not use this PDF as proof of the specific PASS-versus-FAIL contradiction until the exact screenshot/report is identified.

The detailed design output observations include fatigue utilization around 1.65–1.70 (FAIL) and total-load deflection around 56.06–56.28 mm against 51.67 mm allowable (FAIL). These are application-reported results, not independent calculations.
