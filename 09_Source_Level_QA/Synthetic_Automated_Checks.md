# Synthetic Automated Check Matrix

These isolated checks used controlled objects or test caches. They did not run the complete application workflow and do not validate structural design calculations.

| Test ID | Synthetic check | Expected behavior | Observed behavior | Status |
| --- | --- | --- | --- | --- |
| SRC-01 | YAML serialization roundtrip | Values and unknown nested keys survive | Fields, booleans, floats and unknown nested keys retained | PASS |
| SRC-02 | InputDock line edit/combo restoration | Supported widget values restore; unmatched keys remain | Line edit/combo and dictionary behavior checked; checkbox not populated | PARTIAL |
| SRC-03 | DCREngine aggregation | All-pass / any-fail cases aggregate consistently | All pass→PASS; a fail/mixed→FAIL; excluded ID 20 only→NO CHECKS RUN | PASS |
| SRC-04 | Design envelope controlled result | Failing envelope returns FAIL | Controlled failing result returned FAIL | PASS |
| SRC-05 | Executive summary synthetic aggregation | Any relevant failing component reflected in overall status | Deck utilization >1.0 with passing girders still produced overall Pass | FAIL |
| SRC-06 | Custom material mapping | Canonical custom properties reach mapping path and serialize | Tested properties used and survived YAML | PASS |
| SRC-07 | Backend validation comparison | Validation entry points reject the same invalid input | One gate accepted `abc`; OSI validator rejected it | FAIL |
| SRC-10 | YAML malformed-root guards | Invalid roots handled without unhandled parse/type errors | Source-level guards observed; GUI behavior not seen | PARTIAL |

The force resolver is documented separately as [DATA-03](../05_Input_Output_Data_Validation/Force_Resolver.md). The 13 input-validator cases are individually listed in [Input Validation](../01_UI_and_Input_Testing/Input_Validation.md) and the execution registry.
