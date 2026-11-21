# InputDock restoration

| Test ID | Method | Expected | Actual | Status |
| --- | --- | --- | --- | --- |
| SRC-02 | Source-level / synthetic | Valid tested behavior is preserved and invalid cases are handled clearly | Line edit/combo restoration checked; unmatched keys retained; checkbox was not populated. | PARTIAL |

**Procedure:** Synthetic offscreen Qt check of line edit, combo, dictionary replacement and unmatched keys.

**Evidence:** Isolated test was reported in the QA notes/workbook; a standalone test log was not located.

**Limitations:** Widget coverage is incomplete; synthetic only. These checks are not full end-to-end calculation validation.
