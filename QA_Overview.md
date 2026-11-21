# QA Overview

## Purpose

This repository presents a traceable account of software quality testing on the OsdagBridge short-span steel girder bridge module. The focus is user-facing behavior, state consistency, data flow, output presentation, persistence, and report generation.

## Scope

Included areas are UI and input validation, boundary conditions, median/footpath design scenarios, repeated spans, custom steel and concrete properties, `.osi` save/load, result tables and force mapping, CAD and visualization controls, CSV menu behavior, source-level checks, and PDF output QA.

## Evidence classes

| Class | Meaning | Example |
| --- | --- | --- |
| Manual GUI | Interaction and behavior observed in the desktop application | Span boundary behavior; CSV menu click |
| Application output | Values generated/displayed by the application | Reported fatigue and deflection status |
| Source inspection | Behavior inferred from code-path review | QAction without a connected handler |
| Synthetic/offscreen | Isolated controlled objects or caches | Two-girder force resolver cache |
| Independent engineering validation | Not performed | No independent calculations against design standards |

## Navigation

See [the root README](README.md), [execution summary](TEST_EXECUTION_SUMMARY.md), [evidence index](EVIDENCE_INDEX.md), [issue tracker](ISSUE_TRACKER.md), and [final assessment](FINAL_QA_ASSESSMENT.md). Detailed cases are grouped in folders `01_` through `10_`.

## Reading the results

Statuses describe only the recorded test scope. A `PASS` means the observed behavior matched the limited scenario; it does not validate the correctness of structural design calculations. A source-level or synthetic pass does not mean that a complete GUI workflow passed.
