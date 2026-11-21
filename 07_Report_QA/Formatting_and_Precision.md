# Formatting and Precision

| Test ID | Field | Expected | Actual | Status |
| --- | --- | --- | --- | --- |
| REP-05 | Overall bridge width | Human-readable decimal precision | `9.899999999999999` recorded; same value visible in inspected PDF text | PARTIAL (formatting defect observation) |

This is a presentation precision finding. It does not by itself indicate an incorrect internal width calculation. Preserve raw value and report formatting in a retest, and compare with the input geometry. Historical reference #70 is a cross-check only and is not asserted as the same defect.
