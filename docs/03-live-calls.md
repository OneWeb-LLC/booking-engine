# Live Calls and Zero Friction

## Live Call standard

A live person has greater urgency than deferred work. Live Calls include inbound calls, warm transfers, Zero Friction connections, returned calls, and AI-to-human transfers.

## Inbound calls

Inbound routing should identify intent and route by skill rather than by arbitrary individual preference. Minimum intake should be collected before a transfer when practical:

- name;
- phone number;
- email when appropriate;
- reason for call;
- service or product interest;
- critical context.

## Warm transfers

A warm transfer is complete only when:

1. the correct recipient answers;
2. the transferring agent introduces the contact and purpose;
3. relevant context is provided;
4. the call is successfully connected;
5. the transferring agent confirms the connection before leaving.

If the transfer fails, recover the live contact and create the next-best action.

## Zero Friction

Zero Friction converts an eligible signal into an immediate human conversation. It is an acceleration mechanism, not a separate Customer Journey path. Typical triggers include:

- new inbound lead submission;
- explicit call request;
- qualified high-intent action;
- approved recovery or reactivation event.

### Execution

1. Allow the configured synchronization window when the lead may be completing a booking action.
2. Validate consent, calling hours, contact eligibility, and duplicate suppression.
3. Recheck the current Journey phase, path tier, appointments, conversion status, and active objective.
4. Create or retain exactly one active call objective.
5. Attempt the contact call.
6. Recheck the state immediately before the agent bridge.
7. When connected, route to an eligible available agent and present the current Call Brief.
8. Record the outcome, path movement, and next action.

### Dynamic objective

| Current state | Zero Friction objective |
|---|---|
| Captured and not booked | Assist the next valid Convert step |
| Appointment already booked | Confirm, prepare, or identify readiness without re-selling the booking |
| Ready to advance | Enter Expedited: close within authority, use Buy Now when configured, or connect to a Sales Officer |
| Already closed | Suppress sales activity and begin or protect onboarding |

### Failure paths

- **Contact does not answer:** preserve the current valid state and enter the Recovery associated with the failed objective. A booked lead remains booked and must not be mislabeled as Booking Recovery.
- **No agent accepts:** apologize or preserve the connection according to configuration, then enter priority recovery.
- **Call drops:** immediately attempt recovery.
- **Invalid/DND:** suppress further calls and record the result.

Zero Friction failure should normally produce a pooled Call Queue entry—not a personal Assigned Task—unless a specific agent accepts ownership. The Call Brief must reflect the latest objective rather than the workflow's original trigger.
