# OSI Save and Load Roundtrip

| Test ID | Objective | Modified input | Expected | Actual | Status |
| --- | --- | --- | --- | --- | --- |
| OSI-01 | Check whether key values survive save and reopen | Span 32 m; carriageway 9.5 m; spacing 2.70 m; deck thickness 270 mm; self-weight factor 1.10 | Each saved value reappears unchanged | Span/width restored as expected in observed run; spacing reverted to 2.60 m; thickness/factor/location retained | FAIL |

## Procedure and reproducibility

Recorded procedure, reconstructed from notes: modify the listed inputs, save an `.osi`, reopen it and inspect restored values. The girder spacing discrepancy was rechecked after save/reopen and reported as 2.70→2.60 m. The count and exact environment of repeated attempts are not preserved, so no numeric reproducibility rate is claimed.

## Restoration matrix

| Parameter | Saved value | After reopen | Status |
| --- | ---: | ---: | --- |
| Span | 32 m | Restored as expected | PASS for observed run |
| Carriageway width | 9.5 m | Restored as expected | PASS for observed run |
| Girder spacing | 2.70 m | 2.60 m | FAIL |
| Deck thickness | 270 mm | Retained | PASS for observed run |
| Self-weight factor | 1.10 | Retained | PASS for observed run |
| Location | Recorded location | Retained | PASS for observed run |

These parameter outcomes describe one recorded flow and do not guarantee every `.osi` key is restored. See [defect detail](Girder_Spacing_Restoration.md).
