# Lock and Unlock Workflow

| Test ID | Objective | Procedure | Expected | Actual | Status | Evidence |
| --- | --- | --- | --- | --- | --- | --- |
| UI-12 | Confirm designed state can be unlocked for edits and redesigned | Recorded workflow: unlock → edit input → redesign; exact click sequence not preserved | Unlock allows intended edits and next design uses edited state | Workflow tested successfully | PASS | Evidence not located |

The successful workflow demonstrates the recorded edit path only. It does not establish that every downstream output clears or refreshes correctly after every possible input change. A separate source-level concern about stale output after loading `.osi` is documented in [Stale Output Risk](../04_Save_Load_and_State/Stale_Output_Risk.md).
