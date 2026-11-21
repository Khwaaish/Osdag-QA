# Reset Workflow

| Test ID | Objective | Source observation | Runtime observation | Status |
| --- | --- | --- | --- | --- |
| SRC-09 | Check Database → Reset action hookup | QAction is created/added to Database menu; no `triggered.connect` was found in the inspected path | Runtime confirmation pending | FAIL (source-level finding) |

The source note also records that `PlateGirderBridge.reset()` releases backend memory only, while the nearby unlock path clears several UI/output states. This suggests incomplete reset semantics, but should be verified against the exact source revision. No source was modified by the tester.

Evidence: source audit notes reported; no standalone source capture or runtime screenshot located. Do not describe this as an observed runtime click failure.
