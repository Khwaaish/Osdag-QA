# CSV-01 — Save Inputs CSV

| Field | Observation |
| --- | --- |
| Objective | Determine whether the Save Inputs (.csv) menu action opens an export workflow |
| Procedure | Clicked Save Inputs (.csv) from the application menu; exact build and repeated count not preserved |
| Expected | A file dialog or defined export action appears |
| Actual | No dialog appeared |
| Status | FAIL |
| Source check | QAction creation/addition observed without a connected trigger handler |
| Runtime evidence | [Menu screenshot](../13_Screenshot_Archive/1/1%20%281%29.png); post-click state evidence not located |
| Draft reference | #62842 — submission/ID unverified |

The source observation is corroborating evidence, not proof of exact runtime cause unless the source revision matches the runtime build. Issue submission is not confirmed. Retest and capture the click/result state before filing.
