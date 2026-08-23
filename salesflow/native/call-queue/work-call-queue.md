# Salesflow Instruction: Work the Call Queue

- **Roles:** Booking Agent and other queue-eligible agents
- **Work Priority:** Call Queue
- **Last logic review:** 2026-08-23
- **Instruction type:** Native
- **UI verification:** Draft — client verification required

## Outcome

The next eligible pooled call is completed consistently, documented, and routed by its disposition.

## Before you begin

Do not enter the Call Queue when an active appointment, Live Call, or due Assigned Task requires attention.

## Where to go

**Salesflow → Conversations → Manual Actions**

## Steps

1. Open **Conversations → Manual Actions**.
2. Apply only the client-approved queue filters.
3. Confirm the correct work type and eligible team.
4. Click **Let's Start**.
5. Accept the next supplied record; do not select favorites.
6. Read the Call Brief, including purpose, trigger, priority, attempt, last outcome, context, and desired result.
7. Recheck appointments, active conversations, exact-time callbacks, DND, terminal outcomes, and current opportunity state.
8. If the objective is obsolete, do not place the call; use the approved Skip or resolution action and correct the record.
9. If eligible, place the call using the approved number and objective.
10. When the call ends, select one definitive disposition.
11. Complete, Skip, or Re-queue the Manual Action according to the actual outcome and client policy.
12. Add a meaningful note only when durable context was created.
13. Allow the disposition workflow to create the next valid action.
14. Continue until higher-priority work becomes active or the queue is empty.

## If the queue is empty

1. Confirm filters are correct.
2. Notify the Team Manager or Campaign Manager through the approved channel.
3. Do not manufacture duplicate tasks or call records.

## Common mistakes

- Cherry-picking records.
- Calling from an obsolete objective.
- Re-queuing without a disposition.
- Creating an Assigned Task for pooled work.
- Adding an automated-event narrative as a note.
