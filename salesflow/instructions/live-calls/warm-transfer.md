# Salesflow Instruction: Warm-Transfer a Live Call

- **Initiating role:** Booking Agent
- **Receiving role:** Sales Officer
- **Work Priority:** Live Calls
- **Last logic review:** 2026-08-23
- **Salesflow dependency:** Core capability
- **UI verification:** Draft — client verification required

## Ownership rule

The Booking Agent initiates the warm transfer and retains ownership until the Sales Officer answers, receives the handoff context, and accepts the connection. The Sales Officer receives or accepts the warm transfer.

## Outcome

The customer and receiving person are connected with the correct context, and responsibility is explicitly accepted.

## Before you begin

1. Confirm the transfer is necessary and the receiving role is correct.
2. Confirm the receiving person is available when possible.
3. Tell the customer who they are being connected to and why.

## Click-by-click walkthrough

1. While the customer remains on the call, open the dialer's **Transfer** control.
2. Choose **Warm Transfer**.
3. Search for the correct Salesflow user or enter the approved destination number.
4. Start the second call.
5. When the recipient answers, give a concise handoff:
   - customer name;
   - service interest or issue;
   - qualification or current state;
   - what has already happened;
   - desired outcome;
   - material objection, urgency, or promise.
6. Confirm the recipient accepts the call.
7. Use **Patch Call** to connect the customer and recipient.
8. Introduce both parties when the call reconnects.
9. Confirm they can hear each other.
10. Leave the call only after the connection is stable.
11. Record the transfer disposition and update ownership or opportunity state.

## If the transfer fails

1. Return to the customer immediately.
2. Apologize without blaming the recipient or system.
3. Tell the customer that the intended recipient is unavailable and offer the correct appointment.
4. Open the client-approved calendar while the customer remains on the call.
5. Book the appointment with the intended Sales Officer or appropriate receiving role.
6. Confirm the date, time, time zone, purpose, and meeting method with the customer.
7. Confirm the appointment is saved and the configured confirmation was sent.
8. Record the client-approved failed-transfer disposition and the booked appointment outcome.
9. Retain ownership until the appointment is saved and confirmed.

A failed warm transfer does not become generic Call Queue work. The Booking Agent retains ownership and books an appointment with the intended Sales Officer before ending the call.

## Common mistakes

- Using blind transfer for a qualified sales or sensitive support handoff.
- Disconnecting before the recipient answers.
- Transferring without context.
- Assuming ownership moved when the recipient did not accept.
- Ending a failed transfer with only a task, note, or promise to call back instead of booking the appointment.
