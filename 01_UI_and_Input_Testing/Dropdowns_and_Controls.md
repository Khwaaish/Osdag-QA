# Dropdowns and Controls

| Test ID | Control | Objective | Actual result | Status | Evidence |
| --- | --- | --- | --- | --- | --- |
| UI-03 | Dropdowns | Check selected values and state | Selected values examined; not exhaustive | PARTIAL | Evidence not located |
| UI-04 | Project location | Check required selection and state | Location state inconsistency observed after loading baseline | PARTIAL | [Location capture](../QA%20Evidence/qa_reset_after.png); not a complete before/after pair |
| UI-10 | Median/footpath toggles | Observe dependent geometry/load fields | Geometry and load changes recorded | PASS | Scenario evidence partly present in archive |

## Location state note

The baseline `.osi` and design/report retained Panjim, Goa while a later Basic Inputs view showed “Select Location.” The available capture [qa_reset_after.png](../QA%20Evidence/qa_reset_after.png) visibly shows both the “Select Location” control and “Panjim, Goa” label in the same UI state. A fresh blank session reportedly blocked design without location. Precise reproduction steps and current issue status are not established. See [state testing](../04_Save_Load_and_State/README.md) and [issue tracker](../ISSUE_TRACKER.md).
