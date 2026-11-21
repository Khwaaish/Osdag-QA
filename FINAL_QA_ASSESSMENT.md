# Final QA Assessment

## Scope completed

The documented work covers UI and input validation, additional input inventories, baseline and comparative scenarios, custom materials, `.osi` persistence, output display, CAD/graphics controls, CSV actions, source-level checks, and PDF report review.

## What worked in the recorded scenarios

The baseline design completed and produced CAD and Output Dock content. Span values 20 m and 45 m were accepted while 19.99 m and 45.01 m were rejected in the recorded validator path. Median/footpath and 31 m/32 m comparisons showed the recorded geometry/load changes. Custom steel propagation, result-table inspection, synthetic resolver mapping, YAML serialization, status aggregation, and PDF export succeeded in their scoped tests.

## Failures and discrepancies

The most actionable findings are the 2.70 m girder spacing restoration defect, one-decimal material-field precision, unresponsive graphics controls, unresponsive Save Inputs menu, source-confirmed missing Reset handler, report dimension labeling, a backend-vs-OSI validator mismatch, and the self-weight summary/moment discrepancy. The application also reported fatigue and total-load deflection failures in the recorded design output. These are software QA observations, not independent design checks.

The QA notes describe a summary PASS alongside detailed failures. The PDF physically present here instead states “Overall Design Status Fail” in its executive summary. Treat the summary/detail finding as a run/copy reconciliation item until the exact report and UI capture are matched.

## Risks and open questions

- A saved input may not restore all values consistently.
- A source-level stale-output path may be possible; runtime reproduction remains pending.
- A reaction plot label may not match the values displayed in the reaction fields.
- Report completeness and blank wind/seismic fields need verification against applicability and source inputs.
- Load-case changes may not refresh a displayed permanent-load summary.
- Historical issue references may refer to another fork or code revision.

## Recommended next QA work

1. Re-run the spacing roundtrip and capture the exact `.osi`, pre-save values and post-load values.
2. Repeat the self-weight comparison from one baseline, restoring factor 1.00 and comparing every relevant output channel.
3. Match each report finding to a run identifier and inspect the exact pages/screenshots.
4. Reproduce and capture CSV, graphics, location, load-case and reset behaviors on a recorded immutable build.
5. Capture live UI/input dictionary/runtime/output/report snapshots for a single test configuration.
6. Review structural calculations independently with a qualified engineer before drawing engineering conclusions.

## Conclusion

This package provides a useful, evidence-linked record of software behavior and several specific issues that merit retesting. It does not establish comprehensive reliability, structural correctness, or suitability for a particular bridge design.
