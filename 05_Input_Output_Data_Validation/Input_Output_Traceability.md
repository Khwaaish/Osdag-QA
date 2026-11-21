# Input and Output Traceability

## Objective

Check whether user-visible inputs propagate through input state, runtime use, result dictionaries, docks, and reports. Traceability matters because matching labels on screen do not guarantee that a value reached the intended calculation or report field.

| Test ID | Data path | Verification method | Expected | Observed | Status | Evidence |
| --- | --- | --- | --- | --- | --- | --- |
| DATA-01 | UI → input state | Manual/source checks | Entered values represented in input state | Partial targeted mapping; no full live comparison captured | PARTIAL | Evidence not located |
| DATA-01 | Input state → runtime | Source-level mapping checks | Intended values used by runtime objects | Custom material mapping tested; not all fields | PARTIAL | Source test log not located |
| DATA-01 | Runtime → output dictionary/dock | Results inspection | Same-run values/components agree | Reaction and summary consistency concerns | PARTIAL | Screenshot evidence partially present |
| DATA-01 | Output → report | PDF inspection | Report reflects output with correct units/status | Report discrepancies recorded; source/run mismatch caveat | PARTIAL | `08_Reports/run_03_design_report.pdf` |

## Limitation

Synthetic and source checks are not full end-to-end calculation validation. No complete same-run trace table across all layers was captured.
