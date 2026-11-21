# Testing Methodology

## Test design

The work used exploratory, functional, boundary, scenario, comparative, persistence, output, reporting, and source-level techniques. The method for each result is called out in its test documentation to prevent a synthetic check or application-generated result from being mistaken for a complete end-to-end test.

| Method | Purpose | Applied to | Limits |
| --- | --- | --- | --- |
| Exploratory GUI testing | Inventory controls and identify unresponsive behavior | Basic and additional inputs, menus, graphics | Not exhaustive for all controls or states |
| Functional testing | Confirm a workflow responds in a recorded scenario | Baseline design, lock/unlock, CAD generation, report export | A single successful run does not establish broad reliability |
| Input validation | Check rejected, accepted, blank and malformed values | Span and selected input/material fields | Not every field and type combination was covered |
| Boundary value analysis | Exercise exact and just-outside span limits | 19.99, 20, 45, 45.01 m cases | Validator and GUI behavior should remain distinguished |
| Scenario-based testing | Observe dependent geometry and loads | Median and bilateral footpaths | Effects were not independently calculated |
| Comparative testing | Compare output across controlled changes | Span 31/32 m; self-weight factor 1.00/1.10 | Different result channels may not be equally complete |
| Persistence testing | Check save, reopen and restoration | `.osi` spacing, thickness, factor and location | Material GUI restoration remains incomplete |
| State consistency testing | Compare visible state with design/output state | Location, load case, stale-output source risk | Stale-output runtime behavior remains pending |
| Output and report verification | Compare values, units, labels and completeness | Results table, reactions, PDF | No independent structural check oracle |
| Source inspection | Examine targeted handlers, validation and mapping | CSV, reset, custom material, validators | Source findings are not runtime proof unless separately observed |
| Synthetic/offscreen checks | Exercise isolated functions with controlled objects | YAML, InputDock, status aggregation, resolver | Not end-to-end application calculation tests |
| Defect documentation | Record expected/actual, evidence and next steps | Findings and issue-reference index | Issue submission is not assumed |

## Evidence capture and reproducibility

Available captures and artifacts are linked in [EVIDENCE_INDEX.md](EVIDENCE_INDEX.md). The numeric screenshot archive preserves generic filenames and is not fully mapped. Where exact steps were not preserved, documentation labels them as reconstructed from notes. Draft issue numbers are not represented as verified GitHub IDs.

## Engineering boundary

Application outputs are recorded as outputs. No independent engineering analysis was performed; design acceptability and code compliance were not certified.
