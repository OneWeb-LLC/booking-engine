# Custom Field Contract

Planned Booking Engine fields:

| Field | Object | Type | Purpose |
|---|---|---|---|
| Booking Engine Journey Phase | Opportunity | Single select | Campaign, Capture, Convert, Close |
| Booking Engine Milestone | Opportunity | Single select or text | Client-configured step inside the phase |
| Booking Engine Path Tier | Opportunity | Single select | Standard, Assisted, Expedited, Recovery |
| Active Call Objective | Contact or Opportunity | Single select | Single current human call outcome |
| Active Objective Owner Type | Opportunity | Single select | Named user or pooled team |
| Active Objective Due | Opportunity | Date/time | Eligibility and escalation timing |
| Recovery Type | Opportunity | Single select | Named Recovery family |
| Call Purpose | Contact or Opportunity | Single select | Current Call Brief purpose |
| Call Attempt Number | Contact or Opportunity | Number | Cadence control |
| Last Call Outcome | Contact or Opportunity | Text or mapped value | Current retry context |
| Snapshot Version | Contact or Opportunity | Text | Installed behavior version |

## Approval rule

These are contracts, not final API identifiers. The Snapshot build must confirm object scope, native alternatives, allowed values, workflow write ownership, and reporting needs before creating them.
