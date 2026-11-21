# Baseline Design

| Test ID | Objective | Setup | Expected | Observed | Status | Evidence |
| --- | --- | --- | --- | --- | --- | --- |
| DES-01 | Confirm a baseline design workflow produces inspectable outputs | Baseline input configuration; recorded span scenarios include 30 m, later 31 m and 32 m | Design completes or provides clear error; CAD and output views populate | Design completed; CAD generated, Output Dock populated and baseline files saved | PASS | `11_Test_Inputs_OSI/Baseline_30m_Highway_Bridge.osi`; report copy in `08_Reports/` |

## Test setup and procedure

The baseline design used the recorded input configuration. Exact values beyond separately documented inputs are not reconstructed. The documented procedure is reconstructed from notes: open the baseline configuration, run design, inspect CAD and Output Dock, then save baseline files.

## Observations and repeatability

The baseline served as the reference point for later 31 m/32 m and feature comparisons. Successful generation shows that the workflow ran in this setup; it does not validate calculation correctness. Full same-input repeated-run determinism was not established.

## Evidence needed for a future repeat

- Application build/commit identifier and complete input snapshot.
- Same-run Input Dictionary, Output Dictionary, CAD export and report.
- Timestamped run identifiers and before/after state.
