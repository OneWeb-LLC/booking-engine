# Salesflow Instruction: Handle a Zero Friction Call

- **Role:** Booking Agent
- **Journey phase:** Capture or Convert
- **Path tier:** Standard, Expedited, or Recovery according to current state
- **Work Priority:** Live Calls
- **Last logic review:** 2026-08-23
- **Salesflow dependency:** Client-configured Zero Friction routing
- **UI verification:** Draft — client verification required

## Outcome

A fresh eligible signal becomes the strongest valid customer conversation without duplicating or reversing progress.

## Before you begin

Salesflow should validate consent, calling hours, DND, contact eligibility, and duplicate suppression. The agent must still trust the latest visible customer state over the workflow's original trigger.

## Click-by-click walkthrough

1. Accept the incoming agent-side connection.
2. Read the live Call Brief before the customer is bridged.
3. Check whether the lead has already booked, converted, or entered another active interaction.
4. Listen to the whisper or connection context when configured.
5. When connected, introduce yourself and state the relevant reason for calling.
6. Determine the current objective:
   - not booked → complete the next valid Standard Convert step;
   - already booked → confirm, prepare, or protect the appointment;
   - ready to advance → use Expedited movement;
   - already closed → protect onboarding and stop sales activity.
7. For a ready lead, close when authorized; otherwise initiate a warm transfer; if the transfer is not accepted, book the correct appointment.
8. Complete the strongest valid action.
9. Select the definitive disposition and update the opportunity.
10. Resolve any work made obsolete by the result.

## If something goes wrong

- Customer does not answer → preserve current progress and enter the Recovery matching the failed objective.
- No agent can accept → create priority Recovery with an accurate Call Brief.
- Call drops → attempt immediate recovery.
- Invalid number or DND → record the result and suppress invalid outreach.

## Common mistakes

- Re-selling an appointment that is already booked.
- Sending every failed Zero Friction attempt to Booking Recovery.
- Leaving an upcoming sales call active after the lead has closed.
- Treating the original trigger as more accurate than the current record.
