# Salesflow Instruction: Execute a Recovery

- **Roles:** All roles according to ownership
- **Path tier:** Recovery
- **Last logic review:** 2026-08-23
- **Salesflow dependency:** Core records plus client-configured Recovery rules
- **UI verification:** Draft — client verification required

## Outcome

A failed, stalled, or invalid transition is restored to the strongest valid next step or closed with a valid exit.

## Click-by-click walkthrough

1. Identify the exact transition that failed.
2. Verify the customer's current Journey phase, milestone, appointments, opportunity, ownership, consent, and terminal status.
3. Select the matching Recovery family:
   - Activation;
   - Booking;
   - Appointment;
   - Conversion;
   - Payment;
   - Onboarding;
   - Reactivation.
4. Preserve every valid step already completed.
5. Identify the strongest valid destination: Standard, Assisted, Expedited, or valid exit.
6. Select the correct execution object:
   - exact time → Appointment;
   - personal responsibility → Assigned Task;
   - pooled outreach → Call Queue and Call Brief;
   - person available now → Live Call.
7. Set the owner or eligible pooled team, due time, cadence, attempt limit, and success condition.
8. Suppress conflicting workflows and duplicate call objectives.
9. Execute the action and record the outcome.
10. Exit Recovery when success, exhaustion, escalation, DND, disqualification, or another valid terminal condition is reached.

## Guardrails

- A booked lead does not enter Booking Recovery merely because an activation call was unanswered.
- A No Show enters Appointment Recovery.
- An exact-time callback is an appointment.
- Recovery never restarts the customer from the beginning without a valid reason.
- Reactivation must not displace fresh active demand.

## Common mistakes

- Recovering the workflow trigger instead of the customer's current state.
- Keeping multiple active call instructions.
- Assigning pooled work to one person without acceptance.
- Leaving Recovery open indefinitely after the attempt limit is exhausted.
