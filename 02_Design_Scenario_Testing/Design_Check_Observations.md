# Design Check Observations

| Test ID | Observation | Recorded output | Status | Limitation |
| --- | --- | --- | --- | --- |
| DES-06 | Design check summary/cards | 8 checks, 6 passed, 0 failed, overall PASS in a recorded UI capture; only 6 visible cards | NEEDS INVESTIGATION | Missing card names/results are not inferred |
| DES-07 | Deck and steel utilization | Crack control ≈99%; overhang flexure ≈94%; steel stress ≈92–93% | PARTIAL | Application outputs only; not independently recalculated |
| ENG-02 | Fatigue | Utilization ≈1.65–1.70, marked FAIL | FAIL | No independent structural validation |
| ENG-03 | Total-load deflection | 56.06–56.28 mm vs 51.67 mm allowable; marked FAIL | FAIL | No independent structural validation |

The six-visible-card observation does not support inventing details for two missing entries. A separate attached PDF copy reviewed in this package states overall design status “Fail”; that artifact needs reconciliation with the UI capture and test report before claiming an exact report-summary contradiction. These values are software outputs, not engineering verification.
