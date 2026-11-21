# Input Dictionary

| Test ID | Component | Verification method | Expected | Observed | Status |
| --- | --- | --- | --- | --- | --- |
| DATA-01 | User input to Input Dictionary | Source inspection and targeted checks; no full live snapshot comparison | UI values and units appear in matching input state | Some serialization/restoration paths checked; complete live map not captured | PARTIAL |
| SRC-01 | YAML roundtrip | Isolated serialization test | Values and unknown keys survive roundtrip | Fields, booleans, floats and nested unknown keys retained | PASS |

No exact dictionary keys or values are asserted here unless recorded in supplied material. A value surviving YAML serialization proves serialization behavior for that tested object, not that the UI populated the correct key or that the solver used it.
