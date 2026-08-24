# Appointment Recovery

Use when a scheduled commitment is endangered, changed, or missed.

## Triggers

- unconfirmed appointment;
- reschedule request;
- cancellation;
- customer no-show;
- representative no-show;
- technical failure.

## Default execution

Attempt immediate recovery while intent is fresh, identify the failure reason, and reschedule only when the appointment remains the strongest next step.

Appointment Recovery may use Live Calls, an exact-time appointment, or the Call Queue depending on the customer's availability.


## Ownership split

1. **Sales Officer:** records the truthful appointment status and documents the sales outcome, including No Show, Cancelled, Showed, or Invalid.
2. **Booking Agent:** owns confirmation, rescheduling, and rebooking after Appointment Recovery is created.
3. **System:** suppresses obsolete reminders, creates the approved recovery action, and preserves the original appointment context.

The Booking Agent does not conduct the appointment or document the sales outcome. The Sales Officer does not leave a no-show unrecorded for the Booking Agent to infer.
