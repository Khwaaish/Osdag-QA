# Basic Inputs

## Scope

Basic input inspection covered field labels, units, defaults, location, geometry, design options, materials, and the input state used for the observed workflows. An inventory review is not a validation of every legal range or engineering value.

| Test ID | Input area | Observed result | Status |
|---|---|---|---|
| UI-01 | Basic inputs inspection | Fields, labels, units and defaults reviewed. | PASS |
| UI-02 | Additional inputs inventory | Additional input categories were documented. | PASS |
| UI-03 | Dropdown testing | Selected values examined; the option matrix was not exhaustive. | PARTIAL |
| UI-04 | Mandatory location validation | Location state inconsistency was observed; all validation paths were not covered. | PARTIAL |
| UI-05 | Span boundary testing | 20 m and 45 m accepted; 19.99 m and 45.01 m rejected. | PASS |
| UI-06 | Invalid span inputs | Recorded out-of-range values were rejected. | PASS |
| UI-07 | Carriageway width | Width changes tested; complete matrix not documented. | PARTIAL |
| UI-08 | Skew angle | Limited cases examined; complete boundary coverage not evidenced. | PARTIAL |
| UI-09 | Invalid field inputs | Several inputs tested; not every field and input type was covered. | PARTIAL |
| UI-10 | Median and footpath dependency | Geometry and load changes were recorded. | PASS |
| UI-11 | Additional Geometry | Some geometry dialogs modified; systematic coverage incomplete. | PARTIAL |
| UI-12 | Lock/unlock workflow | Unlock, edit and redesign workflow tested. | PASS |

## Inventory

| Input family | Recorded review |
| --- | --- |
| Structure and design | Highway bridge module; design type and material selectors inspected |
| Geometry | Span, carriageway width, skew, median and footpath controls reviewed |
| Location | Location selector observed; a later state inconsistency was recorded |
| Defaults and units | Labels, units and visible defaults reviewed; no complete per-field baseline export located |

## Conclusion

Basic field inventory was recorded. Full field-by-field values and every default are not reproduced here because a verified complete inventory file was not located. See [UI test matrix](Input_Validation.md) for boundary and invalid-input results.
