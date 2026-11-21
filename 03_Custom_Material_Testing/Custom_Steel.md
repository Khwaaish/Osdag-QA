# Custom Steel

| Test ID | Objective | Setup | Actual | Status | Evidence |
| --- | --- | --- | --- | --- | --- |
| MAT-01 | Create and apply a custom steel material | `custom_steel_520_410` examined; user-entered properties | Material entered and applied; custom properties propagated to tested girder/stiffener path | PASS | [Dialog before](../04_Custom_Materials/MAT-01_Custom_Steel_Dialog_Before.png) · [Added](../04_Custom_Materials/MAT-01_Custom_Steel_Added.png) |
| MAT-02 | Check decimal input precision | Affected fields included Poisson ratio/thermal expansion | UI limited input to one decimal in observed fields | FAIL | [Precision screenshot](../04_Custom_Materials/MAT-02_Decimal_Precision_Limit.png) |

| Property | Observed record |
| --- | --- |
| Material key | `custom_steel_520_410` |
| Yield / ultimate strength tested for stress-limit observation | 520 / 410 MPa |
| Elastic modulus / Poisson ratio | 200 GPa / 0.3 |
| Shear modulus displayed | ≈76.9 GPa |
| Density / thermal coefficient in other archived dialog | 76.4 kN/m³ / 11.7 × 10⁻⁶ /°C (visible screenshot shows a separate `custom_steel_250_410` case) |

The screenshot values for `custom_steel_250_410` must not be merged with the 520/410 material case. The one-decimal precision issue is cross-referenced to historical reference #76; its current status was not verified.

## Stress-limit display observation

| Yield strength | Displayed limit | Formula text | QA note |
| ---: | ---: | --- | --- |
| 350 MPa (E350A) | 315 MPa | `Fy/γM0`, with γM0 = 1.10 | Displayed value equals 0.9Fy; formula/value relationship needs clarification |
| 520 MPa (custom) | 468 MPa | `Fy/γM0`, with γM0 = 1.10 | Displayed value equals 0.9Fy; not independently validated |

This is a recorded formula/value discrepancy, not a conclusion about the correct engineering resistance formula.
