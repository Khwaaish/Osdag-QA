# OsdagBridge — Software QA & Testing

This repository documents software quality assurance and testing activities conducted on OsdagBridge, a steel bridge design application. It contains manual GUI test evidence, test inputs, reports, notes, and documented anomalies.

## Testing scope

- UI behavior and input validation, including boundary values
- Structural design scenarios and repeated design runs
- Custom material configuration and propagation
- Input and output data checks, including `.osi` state restoration
- CAD and visualization controls
- PDF report and CSV export behavior
- Defect observations and supporting evidence

## Approach and environment

Testing used manual execution through the application GUI, controlled input changes, output comparisons, report inspection, and targeted source-level verification.

- OS: Windows
- Python: 3.12
- Environment: Conda
- Branch tested: `dev`

## Findings summary

The recorded work examined input validation and boundary behavior, custom material handling, repeated design and `.osi` state restoration, CSV export actions, report consistency, and visualization controls. Reported anomalies include state inconsistencies, unresponsive CSV export actions, and report/output consistency concerns. See the evidence and notes before treating any observation as a confirmed defect; archived screenshots are not all mapped to a specific test.

## Repository contents

| Path | Contents |
| --- | --- |
| `00_START_HERE/` | Package notes and starting guidance |
| `04_Custom_Materials/` | Custom material test evidence |
| `08_Reports/` | PDF reports and report screenshots |
| `09_Anomalies_and_Failures/` | Evidence associated with anomalies and failures |
| `11_Test_Inputs_OSI/` | `.osi` test inputs |
| `12_Test_Logs_and_Notes/` | QA workbook and run logs |
| `13_Screenshot_Archive/` | Preserved screenshot archive; filenames retained |
| `QA Evidence/` | Additional state and reset evidence |

## Limitations

Testing was primarily manual GUI testing with targeted source-level checks. No comprehensive pytest suite was authored or executed. No independent structural engineering validation was performed. This repository is a software QA record, not a certification of structural design correctness.

## Evidence handling

Evidence status should be described as **Manual observed**, **Automated or source check**, or **Potential / needs investigation** as appropriate. The archive is preserved as received; presence of a file does not imply it has been reviewed or linked to a test case.
