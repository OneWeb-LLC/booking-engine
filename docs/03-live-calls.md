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

Zero Friction converts a fresh signal into an immediate human conversation. Typical triggers include:

- new inbound lead submission;
- explicit call request;
- qualified high-intent action;
- approved recovery or reactivation event.

### Execution

1. Validate consent, calling hours, contact eligibility, and duplicate suppression.
2. Attempt the contact call.
3. When connected, route to an eligible available agent.
4. Present a concise live Call Brief.
5. If both sides connect, begin the conversation.
6. Record outcome and next action.

### Failure paths

- **Contact does not answer:** send the configured message and enter Booking Recovery.
- **No agent accepts:** apologize or preserve the connection according to configuration, then enter priority recovery.
- **Call drops:** immediately attempt recovery.
- **Invalid/DND:** suppress further calls and record the result.

Zero Friction failure should normally produce a pooled Call Queue entry—not a personal Assigned Task—unless a specific agent accepts ownership.

