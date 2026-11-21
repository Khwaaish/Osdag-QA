# Test Execution Summary

## Counting rule

The registry counts **79 unique test IDs** documented in this repository. Summary tables and narrative sections reuse those IDs and are not counted again. The 13 input-validator cases are counted separately because each has a distinct recorded input/result. Inventory review is `PARTIAL` because recording the selected values does not establish engineering correctness. One registered case, Save Outputs runtime behavior, is explicitly `NOT TESTED` because it was not clicked in the recorded testing.

## Results by category

| Category | Cases | PASS | FAIL | PARTIAL | NEEDS INVESTIGATION | NOT TESTED |
|---|---|---|---|---|---|---|
| UI and controls | 12 | 6 | 0 | 6 | 0 | 0 |
| Additional input inventories | 6 | 0 | 0 | 6 | 0 | 0 |
| Design scenarios | 7 | 4 | 0 | 1 | 2 | 0 |
| Custom materials | 10 | 3 | 1 | 6 | 0 | 0 |
| OSI persistence | 1 | 0 | 1 | 0 | 0 | 0 |
| Data validation | 3 | 2 | 0 | 1 | 0 | 0 |
| CAD | 2 | 1 | 0 | 1 | 0 | 0 |
| Graphics | 1 | 0 | 1 | 0 | 0 | 0 |
| CSV | 2 | 0 | 1 | 0 | 0 | 1 |
| Reports | 8 | 2 | 2 | 2 | 2 | 0 |
| Reaction consistency | 1 | 0 | 0 | 0 | 1 | 0 |
| Engineering output observations | 3 | 0 | 2 | 1 | 0 | 0 |
| Source-level checks | 10 | 4 | 3 | 2 | 1 | 0 |
| Validator subcases | 13 | 8 | 5 | 0 | 0 | 0 |

## Overall status totals

| Status | Count |
|---|---|
| PASS | 30 |
| FAIL | 16 |
| PARTIAL | 26 |
| NEEDS INVESTIGATION | 6 |
| NOT TESTED | 1 |

These figures are documentation counts, not a pass rate. Runtime GUI tests, source checks, synthetic checks, and validator cases are different evidence classes.

## Runtime GUI work

Recorded manual work includes baseline design, input inventory and span boundaries, median and footpath comparisons, repeated-span comparison, self-weight sensitivity, custom material workflows, `.osi` restoration, results-table review, CAD generation, graphics controls, CSV menu action, and report generation/export. See [UI](01_UI_and_Input_Testing/README.md), [scenarios](02_Design_Scenario_Testing/README.md), [state](04_Save_Load_and_State/README.md), and [report QA](07_Report_QA/README.md).

## Source and synthetic work

Ten targeted source/synthetic records cover YAML roundtrip, InputDock restoration, status aggregation, design-envelope status, synthetic executive summary logic, custom material mapping, backend validation, stale-output risk, reset action hookup, and YAML error handling. Thirteen `.osi` validation inputs are separately recorded. These are focused checks, not end-to-end calculation tests.

## Major failures and investigation items

- **FAIL:** spacing persistence, material decimal precision, graphics controls, Save Inputs, report units, summary/detail observation as recorded in notes, synthetic summary aggregation, backend validation mismatch, reset handler source audit, and recorded fatigue/deflection checks.
- **NEEDS INVESTIGATION:** self-weight sensitivity, report reaction completeness, wind/seismic fields, reaction plot labels, and possible stale output after loading inputs.
- **PARTIAL:** dropdown/input coverage, materials persistence, complete dictionary traceability, and several additional input inventories.

## Planned or unverified work

Save Outputs was not clicked at runtime. A complete three-run GUI material-change sequence, complete UI-to-dictionary trace, full custom-material GUI restore, stale-output runtime reproduction, GUI YAML error handling, and independent structural validation were not documented as completed.
