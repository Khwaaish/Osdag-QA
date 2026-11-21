# Stale Output Risk

| Test ID | Objective | Method | Observation | Status |
| --- | --- | --- | --- | --- |
| SRC-08 | Determine whether loaded inputs invalidate prior design outputs | Source-level inspection | `.osi` load reportedly does not invoke unlock/clear; `OutputDock._require_design` checks lock but not backend/input equality | NEEDS INVESTIGATION |

This is a source-derived risk, not a reproduced GUI defect. The possible impact is that outputs from an earlier design might remain visible after a different input file is loaded. Runtime stale behavior remains pending. Related historical reference #285 is only a cross-check; current status and exact version applicability are unknown.

**Next step:** design once, load a visibly different `.osi`, then inspect whether outputs are invalidated or clearly marked stale before they can be reused/exported. Preserve both inputs and outputs from the same build.
