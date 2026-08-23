# Action: Handle an Inbound Call

## Outcome

The caller reaches a resolution, appointment, conversion, accepted handoff, valid Recovery, or valid exit without losing context or ownership.

## Trigger and owner

Trigger: an eligible inbound call is presented or accepted.  
Owner: the receiving user until resolution or accepted handoff.

## Rules

- Capture a callback number early.
- Review existing state before creating new work.
- Resolve within authority when possible.
- Expedite a qualified ready customer.
- Transfer responsibility only through an accepted handoff.

## Completion and failure

Complete when the caller receives a resolution, appointment, conversion, accepted handoff, Recovery, or valid exit. Recover a dropped call immediately using the verified callback number.

## Salesflow instruction

[Answer an inbound call in Salesflow](../../salesflow/native/live-calls/answer-inbound-call.md)
