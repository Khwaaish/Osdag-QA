# DCREngine status aggregation

| Test ID | Method | Expected | Actual | Status |
| --- | --- | --- | --- | --- |
| SRC-03 | Source-level / synthetic | Valid tested behavior is preserved and invalid cases are handled clearly | PASS; one failure and mixed status yielded FAIL; only excluded check 20 yielded NO CHECKS RUN. | PASS |

**Procedure:** Controlled all-pass, single-fail, mixed and excluded-ID cases.

**Evidence:** Isolated test was reported in the QA notes/workbook; a standalone test log was not located.

**Limitations:** Controlled inputs do not validate all production DCRs. These checks are not full end-to-end calculation validation.
