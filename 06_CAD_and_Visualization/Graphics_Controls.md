# Graphics Controls

| Test ID | Action | Expected | Actual | Status | Evidence |
| --- | --- | --- | --- | --- | --- |
| VIS-01 | Show Front View | Camera switches to front view | Recorded unresponsive | FAIL | [Graphics menu capture](../13_Screenshot_Archive/3/3%20%2818%29.png); click-result capture not located |
| VIS-01 | Show Top View | Camera switches to top view | Recorded unresponsive | FAIL | Same menu screenshot; result capture not located |
| VIS-01 | Show Side View | Camera switches to side view | Recorded unresponsive | FAIL | Same menu screenshot; result capture not located |
| VIS-01 | Rotate 3D Model (Ctrl+R) | Model rotates | Recorded unresponsive | FAIL | Same menu screenshot; result capture not located |

The exact failure mechanism, repeat count, and display/platform dependence were not isolated. The screenshot proves menu labels are present, not by itself that each action failed. Runtime actions are recorded as unresponsive in the QA notes; fresh before/after capture is recommended. Historical reference #53 is an unverified cross-check.
