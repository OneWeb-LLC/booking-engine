# Handoffs

## Definition

A handoff transfers both context and responsibility. Sending a message or changing a pipeline stage alone does not complete a handoff.

## Standard handoff chain

Campaign Manager → Booking Agent → Sales Officer → Onboarding Coordinator → Support Officer

## Required handoff packet

- customer identity;
- current Journey stage;
- reason for handoff;
- relevant context;
- action already taken;
- open concerns or objections;
- expected next outcome;
- new owner or eligible team;
- due time or appointment;
- acceptance status.

## Completion standard

A handoff is complete only when:

1. the correct recipient or team is identified;
2. sufficient context is available;
3. the receiving party accepts responsibility or routing confirms acceptance;
4. the prior owner confirms the transition;
5. failure automatically enters the appropriate recovery.

## Booking Call advancement

For a ready lead, use the strongest valid destination in this order:

1. Booking Agent closes when explicitly authorized.
2. If not authorized, the Booking Agent initiates a warm transfer to an authorized Sales Officer.
3. If the transfer is not accepted, the Booking Agent books the correct appointment before ending the call.

## Live handoff

For sales warm transfers, the Booking Agent initiates the transfer and remains until the Sales Officer answers, receives the handoff context, and explicitly accepts the connection. The Sales Officer receives or accepts the transfer; the Sales Officer does not initiate the Booking Agent's handoff.

If the Sales Officer cannot accept the warm transfer, the Booking Agent retains ownership and books the customer into the correct appointment before ending the call. A task, note, Call Queue entry, or unconfirmed promise to call later does not satisfy the failed-transfer requirement.

## Asynchronous handoff

For tasks and onboarding transitions, ownership, due time, context, and acknowledgment must be recorded. An unaccepted handoff must remain visible to management.
