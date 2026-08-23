# Action: Update an Opportunity

## Outcome

The opportunity accurately represents the customer's phase, milestone, ownership, value, and commercial status.

## Trigger and owner

Trigger: a customer action changes lifecycle state, ownership, value, or terminal status.  
Owner: the user completing the transition or workflow explicitly authorized to update it.

## Rules

- Stage records what has happened, not what an agent hopes will happen.
- Status remains Open until a valid terminal condition occurs.
- Ownership moves only when accepted.
- A pipeline move does not complete a handoff.

## Completion and failure

Complete when the correct opportunity is saved in the truthful stage, status, and ownership state. If the proper state is unclear, do not guess; retain the current state and escalate the ambiguity.

## Salesflow instructions

- [Update an opportunity in Salesflow](../../salesflow/native/opportunities/update-opportunity.md)
- [Use Snapshot pipeline and path fields](../../salesflow/snapshot/path-and-objective-fields.md)
