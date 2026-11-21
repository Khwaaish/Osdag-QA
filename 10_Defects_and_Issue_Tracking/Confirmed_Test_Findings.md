# Confirmed Test Findings

“Confirmed” here means the documented test observation occurred in its stated test class; it does not establish root cause or engineering impact.

| Finding ID | Title | Type | Status | Evidence/submission |
| --- | --- | --- | --- | --- |
| QA-OSI-01 | Girder spacing reverts on `.osi` restore | Manual persistence | FAIL | Test inputs present; issue not submitted/verified |
| MAT-02 | Custom material decimal restriction | Manual UI | FAIL | [Screenshot](../04_Custom_Materials/MAT-02_Decimal_Precision_Limit.png); cross-check #76 |
| CSV-01 | Save Inputs gives no dialog | Manual + source | FAIL | Menu screenshot present; draft #62842 unverified |
| VIS-01 | Four graphics actions unresponsive | Manual observation | FAIL | Menu capture present; post-click states not located |
| SRC-05 | Synthetic summary aggregation discrepancy | Synthetic/source | FAIL | Test log not located |
| SRC-07 | Backend and OSI validator mismatch | Source/targeted | FAIL | Test log not located; downstream impact unverified |
| SRC-09 | Reset action lacks discovered handler | Source-level | FAIL | Runtime pending |
| REP-03 | Unit label/magnitude concern | Report observation | FAIL | Report copy available; exact mapping should be visually checked |
