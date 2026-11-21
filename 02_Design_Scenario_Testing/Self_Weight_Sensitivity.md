# Self-Weight Sensitivity

| Test ID | Objective | Input change | Expected sensitivity | Actual | Status | Evidence |
| --- | --- | --- | --- | --- | --- | --- |
| DES-05 | Observe consistency when changing the self-weight factor | 1.00 → 1.10, then reset to 1.00 and rerun | Relevant self-weight loads and derived responses should update consistently | Permanent load summary changed; SW moment outputs stayed identical | NEEDS INVESTIGATION | `09_Anomalies_and_Failures/RUN-05_SelfWeight_110_Rerun.png`; workbook copies |

## Recorded values

| Factor | Permanent Load Summary | SW maximum moments |
| --- | ---: | --- |
| 1.00 | 28.487 kN/m | G1/G4 205.44 kNm; G2/G3 204.96 kNm |
| 1.10 | 28.761 kN/m | G1/G4 205.44 kNm; G2/G3 204.96 kNm |

## Discrepancy and risk

The summary changes by 0.274 kN/m while the reported SW moment values are identical. This is an output consistency discrepancy. It may indicate a reporting, load mapping, or calculation-path issue, but the observation does not establish which path is wrong or whether the structural calculation is incorrect.

## Follow-up

Repeat from one saved baseline, verify the effective factor in the runtime input state, capture all load and moment outputs from the same run, compare relevant dictionary values, and independently review the calculation path. Check for duplicates in the exact upstream repository before filing an issue.
