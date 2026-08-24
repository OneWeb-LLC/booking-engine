# Salesflow Instruction: Answer an Inbound Call

- **Primary role:** Booking Agent
- **Receiving specialist:** Support Officer when routed or handed off
- **Work Priority:** Live Calls
- **Last logic review:** 2026-08-23
- **Salesflow dependency:** Core capability
- **UI verification:** Draft — client verification required

## Outcome

The caller reaches the correct next outcome without repeating information or losing ownership.

## Click-by-click walkthrough

1. Accept the Salesflow call promptly when you are available.
2. Use the approved greeting and identify the business.
3. Confirm the caller's name and callback number early in the conversation.
4. Find or create the correct contact record without duplicating an existing contact.
5. Identify the reason for the call and the desired outcome.
6. Review current appointments, opportunity status, and recent context before creating new work.
7. Resolve within your authority when possible.
8. If the caller is a qualified ready lead, follow the Booking Call advancement rule:
   - authorized → close now using the approved action;
   - not authorized → initiate a warm transfer to an authorized Sales Officer;
   - transfer not accepted → book the correct appointment before disconnecting.
9. If the lead is not ready to close or transfer but the next valid step is a sales appointment, book the appointment before disconnecting.
10. If another role is required, complete an accepted warm handoff.
11. End the call only after confirming the next step.
12. Select the disposition and update Salesflow immediately.

## Completion standard

The caller received a resolution, appointment, completed conversion, accepted handoff, valid Recovery, or valid exit.

## If something goes wrong

- Call drops → attempt immediate callback using the verified number.
- Warm-transfer recipient unavailable → retain ownership and book the correct appointment before ending the call.
- Wrong department → warm-transfer with context; do not send the caller away blindly.

## Common mistakes

- Transferring before collecting a callback number.
- Asking the caller to repeat information already in Salesflow.
- Creating a duplicate appointment or opportunity.
- Ending without a disposition and next action.
