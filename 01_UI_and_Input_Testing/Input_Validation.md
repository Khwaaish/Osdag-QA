# Input Validation

## Boundary and invalid-input matrix

| Test ID | Test | Expected | Actual | Status | Evidence |
|---|---|---|---|---|---|
| UI-04 | Mandatory location validation | Inputs outside allowed conditions rejected; valid boundary accepted. | Location state inconsistency was observed; all validation paths were not covered. | PARTIAL | Evidence not located |
| UI-05 | Span boundary testing | Inputs outside allowed conditions rejected; valid boundary accepted. | 20 m and 45 m accepted; 19.99 m and 45.01 m rejected. | PASS | Evidence not located |
| UI-06 | Invalid span inputs | Inputs outside allowed conditions rejected; valid boundary accepted. | Recorded out-of-range values were rejected. | PASS | Evidence not located |
| UI-07 | Carriageway width | Inputs outside allowed conditions rejected; valid boundary accepted. | Width changes tested; complete matrix not documented. | PARTIAL | Evidence not located |
| UI-08 | Skew angle | Inputs outside allowed conditions rejected; valid boundary accepted. | Limited cases examined; complete boundary coverage not evidenced. | PARTIAL | Evidence not located |
| UI-09 | Invalid field inputs | Inputs outside allowed conditions rejected; valid boundary accepted. | Several inputs tested; not every field and input type was covered. | PARTIAL | Evidence not located |

## Exact span cases

| Input | Observed behavior | Status |
| --- | --- | --- |
| 19.99 m | Rejected | PASS |
| 20 m | Accepted | PASS |
| 45 m | Accepted | PASS |
| 45.01 m | Rejected | PASS |

The recorded UI span boundary is 20–45 m. Separate source/validator behavior is documented under [YAML and validation QA](../09_Source_Level_QA/README.md); do not treat it as the same test surface. Some invalid field values and blank/nonnumeric validator inputs were exercised, but the full field-by-type matrix was not documented.

## Targeted `.osi` validator cases

These 13 cases are distinct from the recorded GUI boundary test above. `PASS`/`FAIL` here refer to the validator's acceptance behavior against the recorded expectation for the tested case; they do not prove a complete design workflow.

| Test ID | Input case | Validator result | Status |
|---|---|---|---|
| VAL-01 | Empty dictionary | Rejected. | PASS |
| VAL-02 | Missing span | Accepted. | FAIL |
| VAL-03 | Empty span | Accepted. | FAIL |
| VAL-04 | Null span | Accepted. | FAIL |
| VAL-05 | Nonnumeric span | Rejected. | PASS |
| VAL-06 | Numeric-string span | Accepted. | PASS |
| VAL-07 | Negative span | Rejected. | PASS |
| VAL-08 | 19.99 m span | Rejected. | PASS |
| VAL-09 | 20 m span | Accepted. | PASS |
| VAL-10 | 45 m span | Accepted. | PASS |
| VAL-11 | 45.01 m span | Rejected. | PASS |
| VAL-12 | Missing additional input | Accepted in recorded matrix. | FAIL |
| VAL-13 | Nonnumeric additional input | Accepted in recorded matrix. | FAIL |

## Test case details

### UI-05 — Span boundary testing

**Objective:** Check acceptance at the recorded lower and upper span limits and rejection just outside them.

**Testing type:** Manual/validation behavior recorded in the test notes.

**Preconditions:** Span field available in the bridge module.

**Procedure:** Enter 20 m, 45 m, 19.99 m and 45.01 m in the recorded boundary checks. Exact click sequence is reconstructed from notes.

**Expected result:** Boundary values accepted and out-of-range values rejected.

**Actual result:** 20 m and 45 m accepted; 19.99 m and 45.01 m rejected.

**Status:** PASS.

**Evidence:** Evidence not located as a named boundary screenshot.

**Limitations:** No full design run at every boundary was recorded.

**QA conclusion:** The recorded boundary handling matched the expected range for these four cases.
