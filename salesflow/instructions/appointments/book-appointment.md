# Salesflow Instruction: Book an Appointment

- **Roles:** Booking Agent, Sales Officer, Onboarding Coordinator, Support Officer
- **Journey phase:** Convert or post-Close service
- **Path tier:** Standard, Assisted, or Recovery
- **Work Priority:** Active Live Call or Assigned Task
- **Last logic review:** 2026-08-23
- **Salesflow dependency:** Core capability
- **UI verification:** Draft — client verification required

## Outcome

The customer has a valid appointment with the correct type, owner, time, purpose, location, and preparation context.

## Before you begin

- Confirm the customer does not already have the required appointment.
- Confirm the appointment is the strongest valid next step.
- Know the correct calendar and appointment type.
- Confirm the customer's time zone and contact information.

## Where to go

Use either:

- **Salesflow → Calendars → Appointment List View → New Appointment**; or
- the appointment action inside the open contact or opportunity record.

## Click-by-click walkthrough

1. Click **New Appointment** or the appointment action on the record.
2. Select the correct **Calendar**.
3. Select and verify the correct **Contact**.
4. Select the responsible team member when the calendar requires it.
5. Enter the approved appointment title and purpose.
6. Select the date, start time, end time, and displayed time zone.
7. Add the correct meeting method: phone, meeting link, or physical location.
8. Add preparation context required by the person receiving the appointment.
9. Review the details aloud or in writing with the customer.
10. Save the appointment.
11. Confirm it appears in the correct calendar or Appointment List View.
12. Confirm the customer receives the configured confirmation.
13. Resolve duplicate or obsolete booking actions.

## What to enter

| Visible field | What belongs here |
|---|---|
| Calendar | The client-approved calendar for the service and appointment purpose |
| Contact | The verified customer record; never create a duplicate merely to book |
| Assigned user | The person or eligible team that will own the appointment |
| Title | The approved appointment name visible to staff and, when configured, the customer |
| Date and time | The time confirmed with the customer in the displayed time zone |
| Meeting method | The approved phone number, meeting link, or physical location |
| Description or notes | Preparation context needed to conduct the appointment—not a replacement for record documentation |

## Screenshot capture plan

When this procedure is verified for a client, capture:

1. the path to **Calendars → Appointment List View**;
2. the **New Appointment** control;
3. calendar, contact, owner, date, time, and time-zone fields;
4. the location or meeting-method field;
5. the saved appointment in the correct calendar;
6. the confirmation or automation evidence when visible.

Store only the final client-verified screenshots. Number them to match the walkthrough steps.

## Completion standard

An appointment is not complete until it appears in Salesflow and the customer knows the time, time zone, purpose, location, and preparation requirement.

## What happens automatically

Client configuration may send confirmations and reminders, create internal notifications, update pipeline stages, or suppress booking follow-up.

## If something goes wrong

- No valid time → create the approved next action or Booking Recovery.
- Wrong calendar or owner → correct the appointment before ending.
- Duplicate appointment → preserve the valid appointment and resolve the duplicate.
- Appointment no longer needed because the lead advanced → cancel or resolve it according to policy and suppress reminders.

## Common mistakes

- Booking without verifying the time zone.
- Using the wrong calendar.
- Creating a task instead of an exact-time appointment.
- Saving without confirming the appointment appears.
- Leaving an obsolete booking Call Queue action active.
