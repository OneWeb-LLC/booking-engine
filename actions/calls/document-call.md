# Action: Document a Call

## Outcome

The definitive call result drives the correct automation while durable human context remains available.

## Trigger and owner

Trigger: any handled call ends or transfers successfully.  
Owner: the user who handled or last owned the call segment.

## Rules

- One definitive disposition per call.
- Opportunity stage records current lifecycle state.
- Appointment records an exact-time commitment.
- Assigned Task records personal responsibility.
- Call Brief records the purpose of pooled work.
- Note records durable context.

## Completion and failure

Complete when disposition, lifecycle state, next object, ownership, and durable context agree. Missing or contradictory documentation remains the call owner's responsibility.

## Salesflow instructions

- [Document the call in Salesflow](../../salesflow/native/notes-and-dispositions/document-call.md)
- [Use the Snapshot disposition map](../../salesflow/snapshot/use-snapshot-dispositions.md)
