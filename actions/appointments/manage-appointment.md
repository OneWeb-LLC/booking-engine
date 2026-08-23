# Action: Manage an Appointment

## Outcome

The scheduled commitment begins on time, advances the customer, and ends with an accurate status and next action.

## Trigger and owner

Trigger: the appointment enters its preparation window.  
Owner: the appointment owner or explicitly eligible team.

## Rules

- Prepare inside the configured window.
- Begin on time.
- Record appointment attendance separately from the commercial outcome.
- No Show enters Appointment Recovery.
- Suppress reminders when advancement makes the appointment obsolete.

## Completion and failure

Complete when attendance, customer outcome, opportunity state, and next action agree. No Show, cancellation, and invalid appointments enter their configured Appointment Recovery or valid exit.

## Salesflow instruction

[Manage an appointment in Salesflow](../../salesflow/native/appointments/manage-appointment.md)
