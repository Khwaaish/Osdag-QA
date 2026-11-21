# QA-OSI-01 — Girder Spacing Not Retained

| Field | Record |
| --- | --- |
| Category | Save/load persistence |
| Status | FAIL |
| Severity recommendation | Medium (QA assessment only): geometry input is silently changed on reload; formal product severity was not assigned |
| Environment | Windows, Python 3.12, Conda `osdagbridge-env`, branch `dev`; exact app commit not located |
| Existing issue | Historical reference #19 concerns custom-field restoration, but exact overlap is unverified |
| Submission status | No issue submission confirmed |

## Objective and setup

Verify that a saved girder spacing is restored without silent replacement by another value. The recorded modified configuration included span 32 m, carriageway width 9.5 m, spacing 2.70 m, deck thickness 270 mm, and self-weight factor 1.10.

## Steps

1. Set the recorded values. The exact starting state was not preserved.
2. Save the input state as `.osi`.
3. Reopen the saved file and inspect the restored geometry values.
4. Recheck spacing after saving and reopening.

The procedure is reconstructed from testing notes; exact menu sequence is not available.

## Expected and actual

**Expected:** spacing restores as 2.70 m, matching the saved input.

**Actual:** spacing did not restore correctly; it became 2.60 m. Span and carriageway width restored as expected in the observed run; deck thickness, self-weight factor and location were retained.

**Reproducibility:** Notes describe a recheck but do not preserve a run count or full pair of screenshots. Treat as reproduced in recorded testing; repeat to quantify reliability.

## Impact and follow-up

Silent geometry substitution can cause a reopened design to use a different input than the user saved. Retest with before-save UI capture, `.osi` text, after-load UI capture and same-build metadata. Inspect serialization and restoration mapping for the spacing field. Do not claim a root cause until confirmed.

**Evidence:** [Roundtrip input](../11_Test_Inputs_OSI/qa_osi_roundtrip.osi) and [pre-load screenshot](../QA%20Evidence/qa_osi_before_load.png). The `.osi` file is a data artifact; its contents do not alone prove which UI value was displayed.
