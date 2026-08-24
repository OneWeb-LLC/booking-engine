# Booking Agent

## Mission

Convert new interest into the strongest valid next step: a correctly protected appointment, an Expedited conversion, a live Sales Officer handoff, or a clearly owned Recovery.

## Start of shift

1. Sign in to Salesflow and set the correct availability state.
2. Confirm the microphone, headset, and inbound calling are working.
3. Review today's appointments and preparation windows.
4. Open Assigned Tasks and identify due or overdue commitments.
5. Confirm which Sales Officers and specialists are available for warm transfers.
6. When higher-priority work is clear, open the Call Queue.

## Daily operating order

1. **Appointments:** honor active scheduled commitments.
2. **Live Calls:** answer inbound and Zero Friction connections.
3. **Assigned Tasks:** complete due personal responsibilities.
4. **Call Queue:** work the next eligible pooled record.

## Standard Path

- Use the configured combination of automation and normal human effort.
- Perform Lead Activation, Zero Friction, inbound response, minimum intake, qualification, and booking when applicable.
- Identify the lead's service need and immediate obstacle.
- Collect only the information required for the next step.
- Help the lead choose and secure the correct appointment.
- Protect appointments the lead already booked through the configured journey.
- Confirm purpose, time, location, preparation requirements, and the completed booking before ending the interaction.
- Do not restart the booking conversation when the appointment is already valid.

## Expedited Path

- Recognize when the lead can advance beyond the expected next step.
- Complete a configured Buy Now or authorized close when permitted.
- Initiate the warm transfer of the qualified lead to the correct Sales Officer.
- If the Sales Officer cannot accept the warm transfer, book the correct appointment before ending the call.
- Never skip mandatory consent, eligibility, payment, safety, or compliance requirements.
- Resolve future calls, tasks, or appointments made obsolete by the advancement.

## Recovery Path

- Preserve valid progress; never send a booked lead backward into Booking Recovery.
- Use the Recovery matching the failed objective.
- Create a pooled Call Queue action unless a specific agent accepts ownership.
- Schedule exact-time callbacks as appointments, not ordinary tasks.

## Authority

### May complete

- minimum intake and qualification;
- appointment booking, confirmation, and rescheduling;
- approved Booking Agent offers or Buy Now actions;
- initiating warm transfers and routine routing;
- dispositions, pipeline movement, Call Briefs, tasks, and meaningful notes within policy.

### Must hand off

- close actions outside Booking Agent authority → Sales Officer;
- payment or registration exception → Onboarding Coordinator;
- post-sale service need → Support Officer;
- compliance, safety, complaint, or authority exception → Team Manager.

## Completion standard

Before leaving a record:

1. select one definitive disposition;
2. update the opportunity to the true stage and status;
3. create the correct appointment, task, or Recovery action;
4. add a note only when future humans need durable context;
5. confirm obsolete work is suppressed.

## Responsibility map

| Responsibility | Salesflow instruction |
|---|---|
| Start prepared | [Start your shift](../../salesflow/instructions/daily/start-shift.md) |
| Answer inbound demand | [Answer an inbound call](../../salesflow/instructions/live-calls/answer-inbound-call.md) |
| Activate fresh leads | [Handle a Zero Friction call](../../salesflow/instructions/live-calls/handle-zero-friction.md) |
| Secure appointments | [Book an appointment](../../salesflow/instructions/appointments/book-appointment.md) |
| Route ready leads | [Warm-transfer a live call](../../salesflow/instructions/live-calls/warm-transfer.md) |
| Complete personal work | [Work Assigned Tasks](../../salesflow/instructions/assigned-tasks/work-assigned-tasks.md) |
| Work pooled calls | [Work the Call Queue](../../salesflow/instructions/call-queue/work-call-queue.md) |
| Record outcomes | [Document a call](../../salesflow/instructions/notes-and-dispositions/document-call.md) |
| Restore progress | [Execute a Recovery](../../salesflow/instructions/recoveries/execute-recovery.md) |

## Scorecard

- speed-to-lead;
- live-call acceptance;
- meaningful-conversation rate;
- booking rate;
- Expedited advancement and successful-transfer rate;
- disposition and documentation compliance;
- recovery restoration rate.
