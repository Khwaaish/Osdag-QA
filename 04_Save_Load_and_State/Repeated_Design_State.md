# Repeated Design and State Consistency

| Test ID | Test | Result | Status | Evidence |
| --- | --- | --- | --- | --- |
| DES-04 | 31 m vs 32 m geometry comparison | Recorded width, girder spacing, overhang and DL changed as listed in scenario report | PASS | Generic output tables; exact capture map pending |
| UI-04 | Location UI vs design/report | Baseline location retained in design/report while input view later displayed “Select Location” | PARTIAL | [Location capture](../QA%20Evidence/qa_reset_after.png); not a complete state pair |
| SRC-08 | Load `.osi` after design and inspect old output state | Source suggests a possible stale-output path; runtime behavior not tested | NEEDS INVESTIGATION | Source audit reported; log not located |

A complete required three-run sequence—baseline, changed geometry, changed material—was not evidenced. The 31/32 m comparison should not be expanded into that claim.
