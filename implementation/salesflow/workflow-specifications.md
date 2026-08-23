# Salesflow Workflow Specifications

## WF-01 New Lead Activation

Trigger: approved new inbound lead.

1. Validate consent, phone, business hours, DND, duplicates, and terminal stages.
2. Create or update opportunity.
3. Assign according to client routing policy.
4. Send immediate acknowledgment.
5. Attempt Zero Friction when eligible.
6. On failure, create Booking Recovery Call Queue entry and Call Brief.
7. On connection, await disposition and continue accordingly.

## WF-02 Missed Inbound Call

1. Send missed-call acknowledgment.
2. Check for an active live conversation or existing recovery action.
3. Create priority Call Queue entry.
4. Exit upon connection, booking, DND, invalid number, or cadence exhaustion.

## WF-03 Appointment Protection

1. Send confirmation.
2. Create human confirmation call only when required by client configuration.
3. Suppress generic outbound calls during the protected appointment window.
4. On completion, trigger disposition-based next steps.
5. On no-show, enter No-Show Recovery.

## WF-04 Assigned Callback

If an exact time is promised, create an appointment owned by the responsible user. Do not create only a generic task.

## WF-05 Call Queue Retry

Trigger: call disposition.

- No Answer/Voicemail/Busy: increment attempt, calculate next due time, and re-enroll if eligible.
- Callback Scheduled: create appointment and suppress pooled calls until resolved.
- Follow-Up Required: create appropriate owned task or future queue record.
- Booked/Won/DND/Disqualified/Wrong Number: exit active call workflows.

## WF-06 Reactivation

1. Validate segment approval and consent.
2. Exclude active opportunities, upcoming appointments, DND, recent contact, and conflicting workflows.
3. Enroll within allowed capacity.
4. Prefer queue pacing over flooding the team.

## Universal pre-enrollment checks

- valid callable number;
- permitted calling time;
- contact consent and DND;
- no active appointment conflict;
- no active Live Call;
- no owned exact-time callback;
- no duplicate Manual Action;
- no terminal disposition;
- attempt limit not exceeded.

