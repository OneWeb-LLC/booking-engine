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

- Protect appointments the lead booked through the configured journey.
- Confirm purpose, time, location, and preparation requirements.
- Do not restart the booking conversation when the appointment is already valid.

## Assisted Path

- Identify the lead's service need and immediate obstacle.
- Collect only the information required for the next step.
- Help the lead choose and secure the correct appointment.
- Confirm the booking before ending the interaction.

## Expedited Path

- Recognize when the lead can advance beyond the expected next step.
- Complete a configured Buy Now or authorized close when permitted.
- Otherwise warm-transfer the qualified lead to the correct Sales Officer.
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
- warm transfer and routine routing;
- dispositions, pipeline movement, Call Briefs, tasks, and meaningful notes within policy.

### Must hand off

- close actions outside Booking Agent authority → Sales Officer;
- payment or registration exception → Onboarding Coordinator;
- post-sale service need → Support Representative;
- compliance, safety, complaint, or authority exception → Team Manager.

## Completion standard

Before leaving a record:

1. select one definitive disposition;
2. update the opportunity to the true stage and status;
3. create the correct appointment, task, or Recovery action;
4. add a note only when future humans need durable context;
5. confirm obsolete work is suppressed.

## Responsibility map

| Responsibility | Action standard | Salesflow instruction |
|---|---|---|
| Start prepared | [Start a shift](../../actions/daily/start-shift.md) | [Start in Salesflow](../../salesflow/native/daily/start-shift.md) |
| Answer inbound demand | [Handle an inbound call](../../actions/calls/handle-inbound-call.md) | [Answer in Salesflow](../../salesflow/native/live-calls/answer-inbound-call.md) |
| Activate fresh leads | [Activate a fresh lead](../../actions/calls/activate-lead.md) | [Handle Zero Friction](../../salesflow/native/live-calls/handle-zero-friction.md) |
| Secure appointments | [Book an appointment](../../actions/appointments/book-appointment.md) | [Book in Salesflow](../../salesflow/native/appointments/book-appointment.md) |
| Route ready leads | [Warm-transfer a customer](../../actions/calls/warm-transfer.md) | [Warm-transfer in Salesflow](../../salesflow/native/live-calls/warm-transfer.md) |
| Complete personal work | [Complete an Assigned Task](../../actions/work/complete-assigned-task.md) | [Work Salesflow Tasks](../../salesflow/native/assigned-tasks/work-assigned-tasks.md) |
| Work pooled calls | [Work pooled calls](../../actions/work/work-call-queue.md) | [Work Manual Actions](../../salesflow/native/call-queue/work-call-queue.md) |
| Record outcomes | [Document a call](../../actions/calls/document-call.md) | [Document in Salesflow](../../salesflow/native/notes-and-dispositions/document-call.md) |
| Restore progress | [Restore broken progress](../../actions/recoveries/restore-progress.md) | [Execute Recovery](../../salesflow/native/recoveries/execute-recovery.md) |

## Scorecard

- speed-to-lead;
- live-call acceptance;
- meaningful-conversation rate;
- booking rate;
- Expedited advancement and successful-transfer rate;
- disposition and documentation compliance;
- recovery restoration rate.
