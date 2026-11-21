# Executive summary aggregation synthetic check

| Test ID | Method | Expected | Actual | Status |
| --- | --- | --- | --- | --- |
| SRC-05 | Source-level / synthetic | Valid tested behavior is preserved and invalid cases are handled clearly | Girder FAIL yielded “Fail (Flexure)”; deck utilization >1.0 with girders passing still yielded overall “Pass”. | FAIL |

**Procedure:** Synthetic girder/deck result combinations.

**Evidence:** Isolated test was reported in the QA notes/workbook; a standalone test log was not located.

**Limitations:** Synthetic discrepancy; overlaps report/UI status observation. These checks are not full end-to-end calculation validation.
