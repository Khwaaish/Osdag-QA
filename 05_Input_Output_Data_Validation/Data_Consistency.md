# Data Consistency

| Test ID | Consistency check | Observed | Status | Follow-up |
| --- | --- | --- | --- | --- |
| DATA-01 | UI vs loaded location | Basic Inputs later showed “Select Location” while design/report retained Panjim, Goa | PARTIAL | Capture exact save/load state pair |
| GIR-01 | Reaction values vs plot | RA 36.11, RB 26.02; plot labels appeared both 36.1 kN | NEEDS INVESTIGATION | Confirm plot endpoint mapping/value source |
| DES-05 | Self-weight summary vs SW moments | Permanent load changed; moments did not | NEEDS INVESTIGATION | Compare run-matched raw outputs |
| REP-02 | UI/test notes vs included report | Notes say summary PASS; included PDF executive summary says Fail | NEEDS INVESTIGATION | Reconcile report/run copies |
| SRC-08 | Loaded inputs vs existing output state | Possible stale state from source review only | NEEDS INVESTIGATION | Runtime reproduction pending |

No independent engineering calculation was performed for these consistency observations.
