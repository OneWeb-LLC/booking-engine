# Snapshot Instruction: Use a Call Brief

- **Instruction type:** Snapshot
- **UI verification:** Planned — verify after Snapshot installation

## Outcome

The agent understands why the call exists, what has already happened, and the strongest valid desired outcome before dialing or accepting a connection.

## Read in this order

1. **Call Purpose**
2. **Trigger**
3. **Current Journey Phase and Milestone**
4. **Current Path Tier**
5. **Active Objective**
6. **Priority and Due Time**
7. **Attempt Number and Last Outcome**
8. **Relevant Context**
9. **Desired Outcome**
10. **Next-Action Rule**

## Rules

- Current customer state overrides the original trigger.
- Recheck appointments, conversion status, active calls, and owned callbacks.
- Do not place a call from an obsolete brief.
- Do not use notes as a substitute for the active Call Brief.

## Snapshot dependencies

See [Custom Fields](../../snapshot/fields/custom.md) and [Workflow Catalog](../../snapshot/workflows/README.md).
