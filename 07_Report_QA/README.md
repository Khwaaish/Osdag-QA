# Report QA

The report test suite examines generation, export, completeness, units, precision, page numbering and status presentation.

| Test ID | Area | Status | Detail |
|---|---|---|---|
| REP-01 | Report generation | PASS | [Report generation](Report_Generation.md) |
| REP-02 | Summary/detail consistency | FAIL | [Summary/detail consistency](Summary_vs_Detailed_Checks.md) |
| REP-03 | Units and dimensions | FAIL | [Units and dimensions](Units_and_Dimensions.md) |
| REP-04 | Support reaction completeness | NEEDS INVESTIGATION | [Support reaction completeness](Load_Completeness.md) |
| REP-05 | Bridge width precision | PARTIAL | [Bridge width precision](Formatting_and_Precision.md) |
| REP-06 | Wind/seismic fields | NEEDS INVESTIGATION | [Wind/seismic fields](Wind_Seismic_Fields.md) |
| REP-07 | PDF page numbering | PARTIAL | [PDF page numbering](PDF_Export_and_Pagination.md) |
| REP-08 | PDF export | PASS | [PDF export](PDF_Export_and_Pagination.md) |

The included report `08_Reports/run_03_design_report.pdf` is 57 physical pages and prints through page 56. QA notes and the attached PDF differ on the executive summary status; see [summary consistency](Summary_vs_Detailed_Checks.md).
