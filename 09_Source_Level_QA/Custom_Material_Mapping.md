# Custom material mapping

| Test ID | Method | Expected | Actual | Status |
| --- | --- | --- | --- | --- |
| SRC-06 | Source-level / synthetic | Valid tested behavior is preserved and invalid cases are handled clearly | Unknown grades/canonical custom keys used in checked path; custom values survived YAML. | PASS |

**Procedure:** Inspected PlateGirderBridge material mapping and YAML path.

**Evidence:** Isolated test was reported in the QA notes/workbook; a standalone test log was not located.

**Limitations:** UI cache `_material_custom_fields` not equivalent to all material persistence behavior. These checks are not full end-to-end calculation validation.
