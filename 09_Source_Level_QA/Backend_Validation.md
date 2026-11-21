# Backend validation inconsistency

| Test ID | Method | Expected | Actual | Status |
| --- | --- | --- | --- | --- |
| SRC-07 | Source-level / synthetic | Valid tested behavior is preserved and invalid cases are handled clearly | “abc” custom wind drag coefficient accepted by one gate and rejected by the other. | FAIL |

**Procedure:** Compared `set_input` + `_validate_inputs` with `validate_osi_inputs`.

**Evidence:** Isolated test was reported in the QA notes/workbook; a standalone test log was not located.

**Limitations:** Calculation impact was not verified. These checks are not full end-to-end calculation validation.
