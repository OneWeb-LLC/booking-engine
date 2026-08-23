# Procedure: Document a Call

- **Roles:** All calling roles
- **Last logic review:** 2026-08-23
- **UI verification:** Draft — client verification required

## Outcome

The definitive call result drives the correct automation, while meaningful context remains available to the next human.

## Steps

1. When the call ends, select exactly one client-approved **Call Disposition** that best represents the definitive outcome.
2. If the customer state changed, update the opportunity stage and status.
3. If an exact-time commitment was made, create the appointment before leaving the record.
4. If a specific person owns additional work, create or update the Assigned Task.
5. If pooled outreach remains, allow the disposition workflow to create or re-queue the Call Queue action.
6. Add a note only when the next human needs durable context not expressed by the disposition, stage, appointment, or task.
7. Resolve obsolete actions created by the prior customer state.

## What belongs where

| Information | Salesflow object |
|---|---|
| Definitive call outcome | Disposition |
| Current lifecycle position | Opportunity stage/status |
| Exact-time commitment | Appointment |
| Personal responsibility | Assigned Task |
| Pooled call purpose | Call Brief |
| Durable human context | Note |

## Expedited documentation

Record the prior stage, destination, advancement reason, authority or method used, and any intentionally skipped milestone. Confirm all skipped milestones were marked skippable or were not applicable.

## Common mistakes

- Choosing multiple or contradictory outcomes.
- Writing a note instead of updating the pipeline.
- Writing “called, no answer” as a permanent narrative note when the disposition already records it.
- Leaving a future appointment active after the customer has already closed.
