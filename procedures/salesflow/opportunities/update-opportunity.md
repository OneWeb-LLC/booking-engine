# Procedure: Update an Opportunity

- **Roles:** Booking Agent, Sales Officer, Onboarding Coordinator, Campaign Manager
- **Journey phase:** Capture, Convert, or Close
- **Last logic review:** 2026-08-23
- **UI verification:** Draft — client verification required

## Outcome

The opportunity accurately represents the customer's current phase, milestone, ownership, value, and commercial status.

## Where to go

**Salesflow → Opportunities → Pipelines**

## Steps

1. Open **Opportunities** and select the correct pipeline.
2. Search for and open the customer's opportunity.
3. Verify the contact identity and service before editing.
4. Review the current stage, status, owner, value, source, appointments, tasks, and recent context.
5. Move the opportunity to the client-approved stage that reflects what has actually happened.
6. Set the truthful opportunity status:
   - **Open:** valid active opportunity;
   - **Won:** customer commitment meets the configured Close standard;
   - **Lost:** decision ended unsuccessfully with a recorded reason;
   - **Abandoned:** client policy authorizes that terminal state.
7. Update the owner only when responsibility has been accepted.
8. Update value or source only from verified information.
9. Save and confirm the card appears in the expected stage.
10. Confirm connected workflows created or suppressed the correct work.

## Guardrails

- Pipeline stage is the customer state, not an agent reminder.
- A task does not replace a stage update.
- Moving a card does not complete a handoff.
- Do not mark Won merely because an appointment was booked.
- Do not mark Lost merely because a call was unanswered.

## Common mistakes

- Moving the wrong opportunity for a contact with multiple services.
- Changing ownership without acceptance.
- Advancing based on intention instead of completed customer action.
- Failing to record a Lost reason.
