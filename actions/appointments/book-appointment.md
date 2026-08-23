# Action: Book an Appointment

## Outcome

The customer has a valid appointment with the correct type, owner, time, purpose, location, and preparation context.

## Trigger and owner

Trigger: an appointment is the strongest valid next commitment.  
Owner: the user securing the appointment until calendar ownership is confirmed.

## Rules

- Confirm no valid duplicate exists.
- Use the correct calendar and time zone.
- Confirm the appointment with the customer.
- Resolve obsolete booking work.
- Do not book an unnecessary appointment when valid Expedited advancement is available.

## Completion and failure

Complete when the appointment is saved, visible, correctly owned, and confirmed with the customer. If no valid time is available, create the approved Assisted or Recovery action.

## Salesflow instruction

[Book an appointment in Salesflow](../../salesflow/native/appointments/book-appointment.md)
