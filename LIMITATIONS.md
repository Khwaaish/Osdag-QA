# Testing Limitations

| Limitation | Effect on conclusions | Follow-up |
| --- | --- | --- |
| Primarily manual GUI activity | Coverage varies by field and workflow | Repeat with controlled case sheets and saved inputs |
| No comprehensive pytest suite authored or run | No broad automated regression claim | Build and execute a separate approved test suite |
| Pytest unavailable in recorded environment | No pytest validation | Install in a controlled test environment if authorized |
| Targeted source/synthetic checks only | Does not prove full application behavior | Pair with runtime tests using the same inputs |
| No independent structural engineering validation | Cannot certify calculations or code compliance | Qualified engineer to review inputs, assumptions and calculations |
| Exact application commit not recorded | Build-specific reproducibility is limited | Record immutable commit and app version for retests |
| Evidence archive uses generic names | Some screenshots cannot be tied to a particular test | Map verified captures to test IDs; do not infer from numbering |
| Some described captures/logs are absent | Some findings are supported by notes only | Capture fresh reproduction evidence |
| Exact duplicate intake copies were deduplicated | Earlier versions remain in repository history | Use canonical evidence index entries |
| One `.png` file is undecodable | It cannot support a visual finding | Recover original screenshot if available |
| Report and QA notes differ on summary status | Exact report/run association is uncertain | Reconcile run ID, report copy and summary field |
| Issue references are not all verified in target fork | Status and ownership cannot be claimed | Check exact repository before citing/submitting |
