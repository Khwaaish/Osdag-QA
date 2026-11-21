# OsdagBridge — Software QA & Testing

This repository is a documented software QA record for the **OsdagBridge short-span steel girder bridge module**. It contains manual GUI observations, scenario comparisons, persistence checks, source-level and synthetic findings, report review, and the supporting evidence files available in this workspace. No OsdagBridge source code was developed or modified as part of this QA work.

## Contents

- [QA overview](QA_Overview.md) · [Methodology](TESTING_METHODOLOGY.md) · [Environment](ENVIRONMENT.md)
- [Execution summary](TEST_EXECUTION_SUMMARY.md) · [Status legend](TEST_STATUS_LEGEND.md) · [Final assessment](FINAL_QA_ASSESSMENT.md)
- [Evidence index](EVIDENCE_INDEX.md) · [Issue tracker](ISSUE_TRACKER.md) · [Limitations](LIMITATIONS.md)

## Project under test

OsdagBridge is a desktop application for short-span steel girder bridge design. The QA scope covered inputs and validation, geometry and design scenarios, custom materials, state and `.osi` persistence, result display and traceability, CAD/graphics controls, CSV menu actions, and report generation.

## Testing approach and environment

Testing combined manual GUI activity, controlled input changes, cross-scenario comparisons, report inspection, source inspection, and targeted synthetic/offscreen checks. Test conclusions distinguish these methods; synthetic checks are not full end-to-end application calculations.

| Item | Recorded environment |
| --- | --- |
| Operating system | Windows |
| Python | 3.12 |
| Environment manager | Conda; environment name `osdagbridge-env` |
| Tested branch | `dev` |
| Application launch command | `conda activate osdagbridge-env`, then `python -m osdagbridge.desktop` from the OsdagBridge source checkout |
| Source changes by tester | None |

## Execution snapshot

The documentation registry contains **79 unique test records** across runtime, source/synthetic, and input-validator categories. Status totals are reported without combining these different testing types into a pass rate.

| Status | Count |
|---|---|
| PASS | 30 |
| FAIL | 16 |
| PARTIAL | 26 |
| NEEDS INVESTIGATION | 6 |
| NOT TESTED | 1 |

These counts summarize documented records, not structural-design correctness or comprehensive product coverage. See [TEST_EXECUTION_SUMMARY.md](TEST_EXECUTION_SUMMARY.md) for category totals and the counting rule.

## Key findings

- `.osi` restoration did not retain the tested 2.70 m girder spacing; it returned as 2.60 m after save and reopen.
- Changing the self-weight factor from 1.00 to 1.10 changed the permanent load summary from 28.487 to 28.761 kN/m while the recorded SW moments remained unchanged. This is a consistency concern, not proof of an incorrect structural calculation.
- Save Inputs produced no dialog; source inspection found menu action creation without a connected trigger. Save Outputs runtime behavior was not tested.
- Four graphics actions were recorded as unresponsive.
- The QA notes record several report and summary inconsistencies. The included report copy itself says “Overall Design Status Fail”; therefore the specific PASS-versus-FAIL summary observation needs run/copy reconciliation.
- The reaction fields and plot labels were inconsistent in the recorded observation. The exact issue scope and underlying value need investigation.

## Coverage navigation

| Area | Documentation |
| --- | --- |
| UI, inputs and validation | [01_UI_and_Input_Testing](01_UI_and_Input_Testing/README.md) |
| Design scenarios | [02_Design_Scenario_Testing](02_Design_Scenario_Testing/README.md) |
| Custom materials | [03_Custom_Material_Testing](03_Custom_Material_Testing/README.md) |
| Save/load and state | [04_Save_Load_and_State](04_Save_Load_and_State/README.md) |
| Input/output data | [05_Input_Output_Data_Validation](05_Input_Output_Data_Validation/README.md) |
| CAD and visualization | [06_CAD_and_Visualization](06_CAD_and_Visualization/README.md) |
| Report QA | [07_Report_QA](07_Report_QA/README.md) |
| CSV and menu actions | [08_CSV_and_Menu_Functionality](08_CSV_and_Menu_Functionality/README.md) |
| Source-level QA | [09_Source_Level_QA](09_Source_Level_QA/README.md) |
| Defects and issue references | [10_Defects_and_Issue_Tracking](10_Defects_and_Issue_Tracking/README.md) |
| Test inputs, evidence and appendices | [11_Test_Inputs](11_Test_Inputs/README.md) · [12_Evidence](12_Evidence/README.md) · [13_Appendices](13_Appendices/README.md) |

## Evidence policy

Evidence links point only to files present in the repository. The screenshot archive contains generically named files that are not all mapped to a test. One file in `QA Evidence/` with a `.png` extension could not be decoded as PNG; it is indexed as unreadable and should be replaced only if an original capture is available. Exact duplicate copies from the intake package were removed from the current tree; earlier copies remain recoverable in Git history.

## Limitations and conclusion

Testing was primarily manual GUI work with targeted source-level and synthetic checks. No comprehensive pytest suite was authored or run; pytest was unavailable during the recorded source QA activity. There was no independent structural engineering validation. This repository records software behavior and report observations and is not a certification of design correctness. The final assessment is [here](FINAL_QA_ASSESSMENT.md).
