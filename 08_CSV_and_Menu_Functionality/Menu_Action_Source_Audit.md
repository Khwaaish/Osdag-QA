# Menu Action Source Audit

| Test ID | Action | Source observation | Runtime observation | Status |
| --- | --- | --- | --- | --- |
| CSV-01 | Save Inputs | QAction created/added; no handler connection located | Click produced no dialog | FAIL |
| CSV-02 | Save Outputs runtime | Similar disconnected wiring suspected by source review | Not clicked | NOT TESTED |
| SRC-09 | Database Reset | QAction present; no trigger handler found | Runtime confirmation pending | FAIL (source-level) |

The source checkout/commit and line references are not included in this repository. No source code was copied or modified. Source findings should be rechecked against the exact version before treating them as current.
