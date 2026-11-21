# Material Persistence

| Test ID | Persistence stage | Actual result | Status |
| --- | --- | --- | --- |
| MAT-09 | Save/load custom properties | Isolated source-level mapping/serialization was checked; full GUI restoration incomplete | PARTIAL |
| MAT-10 | Change material between designs | Source-level checks only; three-run GUI persistence not verified | PARTIAL |

| Property path | Evidence class | What was checked | Not established |
| --- | --- | --- | --- |
| YAML custom-property roundtrip | Synthetic/source | Tested mapping values survived serialization | Full UI dialog restoration |
| Material after `.osi` load | Not complete | A known UI cache field is referenced in historical issue #19 | Current behavior and issue status |
| Material change after unlock/redesign | Source-level | Mapping path inspected | Full three-run GUI result propagation |

Future retest should preserve a before-save `.osi`, reopened `.osi`, material dialog values, input dictionary, and output properties for the same build.
