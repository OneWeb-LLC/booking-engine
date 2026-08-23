# Action: Restore Broken Progress

## Outcome

A failed, stalled, or invalid transition is restored to the strongest valid next step or closed with a valid exit.

## Trigger and owner

Trigger: a required transition fails, stalls, or becomes invalid.  
Owner: the named Recovery owner or explicitly eligible pooled team.

## Rules

- Recover the current customer state, not the original workflow trigger.
- Preserve every valid completed milestone.
- Select the matching Recovery family.
- Use the correct execution object and owner.
- Suppress collisions and exit Recovery at success, exhaustion, escalation, or valid termination.

## Completion and failure

Complete when the customer rejoins a valid path or reaches a valid exit. Exhaustion without a defined terminal or escalation state is a system defect.

## Salesflow instructions

- [Execute a Recovery in Salesflow](../../salesflow/native/recoveries/execute-recovery.md)
- [Use Snapshot Recovery fields](../../salesflow/snapshot/path-and-objective-fields.md)
