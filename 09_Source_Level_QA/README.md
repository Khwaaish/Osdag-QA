# Source-Level QA

This section contains targeted source checks and synthetic/offscreen checks. None should be described as full end-to-end application tests.

| Test ID | Check | Status | Detail |
|---|---|---|---|
| SRC-01 | YAML serialization roundtrip | PASS | [YAML serialization roundtrip](YAML_Roundtrip.md) |
| SRC-02 | InputDock restoration | PARTIAL | [InputDock restoration](InputDock_Restoration.md) |
| SRC-03 | DCREngine status aggregation | PASS | [DCREngine status aggregation](DCREngine_Status_Aggregation.md) |
| SRC-04 | Design envelope controlled result | PASS | [Design envelope controlled result](Design_Envelope_Check.md) |
| SRC-05 | Executive summary aggregation synthetic check | FAIL | [Executive summary aggregation synthetic check](Executive_Summary_Aggregation.md) |
| SRC-06 | Custom material mapping | PASS | [Custom material mapping](Custom_Material_Mapping.md) |
| SRC-07 | Backend validation inconsistency | FAIL | [Backend validation inconsistency](Backend_Validation.md) |
| SRC-08 | Stale output source risk | NEEDS INVESTIGATION | [Stale output source risk](Stale_Output_Risk.md) |
| SRC-09 | Reset menu action source audit | FAIL | [Reset menu action source audit](Reset_Action.md) |
| SRC-10 | YAML error handling | PARTIAL | [YAML error handling](YAML_Error_Handling.md) |

**Source-level testing limitations:** synthetic inputs exercise only the selected function/object path. No comprehensive pytest suite was authored or run; pytest was unavailable in the recorded environment. No application source code is included in this QA repository.
