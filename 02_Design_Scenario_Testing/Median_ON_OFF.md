# Median ON and OFF Comparison

| Test ID | Objective | Configuration | Observed result | Status | Evidence |
| --- | --- | --- | --- | --- | --- |
| DES-02 | Check median geometry/load dependency | Four girders; median ON dimensions recorded below; compare median OFF | Geometry and load response changed in recorded comparison | PASS | Generic archive includes related output tables; exact screenshots are not individually confirmed |

## ON/OFF values

| Metric | Median ON | Median OFF |
| --- | ---: | ---: |
| Overall width | 20.10 m | Not recorded |
| Girder spacing | 5.03 m | Not recorded |
| Overhang | 2.51 m | Not recorded |
| Number of girders | 4 | Not recorded |
| Median width / height | 1.2 m / 0.9 m | Disabled |
| Median area / density | 0.5632 m² / 25 kN/m³ | Disabled |
| Median load | 14.08 kN/m | Disabled |
| DL | 51.276 | 28.631 |
| SW BM | Approximately 230 kNm | Not recorded |
| DD BM | Approximately 2525 kNm | Approximately 1251.74 |
| Shear | Approximately 554 kN | Approximately 220.31 |

Units for DL were not stated in the supplied scenario note; the values are reproduced as recorded without assigning a unit. Other output values are approximate as supplied.

## Interpretation and limits

Turning the median on coincided with a higher recorded permanent-load value and a change in output geometry. The test supports the expected directional dependency in the observed case. It does not isolate the median contribution using an independent load calculation or establish that every related output is correct.

## Evidence checklist

- Evidence not located for matched ON/OFF input and output snapshots.
- Future retest should preserve both `.osi` states, full output tables and CAD from the same software build.
