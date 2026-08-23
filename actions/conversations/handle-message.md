# Action: Handle a Customer Message

## Outcome

The customer's message is understood, correctly owned, answered, and converted into the strongest valid next action.

## Trigger and owner

Trigger: a new or unresolved customer message becomes eligible.  
Owner: the assigned user or explicitly eligible inbox team.

## Rules

- Verify identity and current Journey state before replying.
- Preserve live momentum when the customer is available now.
- An exact-time promise becomes an appointment.
- Personal responsibility becomes an Assigned Task.
- Do not mark handled until a response or accepted owner exists.

## Completion and failure

Complete when the customer has a response and a valid next state or accepted owner. If the message cannot be handled, create the correct personal action or escalation; never hide it by marking it read.

## Salesflow instruction

[Manage the Salesflow Conversations inbox](../../salesflow/native/conversations/manage-inbox.md)
