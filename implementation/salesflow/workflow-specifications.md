# Salesflow Workflow Specifications

## WF-01 New Lead Activation

Trigger: approved new inbound lead.

1. Validate consent, phone, business hours, DND, duplicates, and terminal stages.
2. Create or update opportunity.
3. Assign according to client routing policy.
4. Send immediate acknowledgment.
5. Allow the configured booking synchronization window.
6. Determine the current Journey phase, path tier, and strongest valid objective.
7. Attempt Zero Friction when eligible.
8. Recheck state immediately before the agent bridge and cancel any obsolete objective.
9. On failure, preserve valid progress and enter the Recovery associated with the failed objective.
10. On connection, continue through Standard, Assisted, or Expedited according to readiness.

## WF-02 Missed Inbound Call

1. Send missed-call acknowledgment.
2. Check for an active live conversation or existing recovery action.
3. Create priority Call Queue entry.
4. Exit upon connection, booking, DND, invalid number, or cadence exhaustion.

## WF-03 Appointment Protection

1. Send confirmation.
2. Create human confirmation call only when required by client configuration.
3. Suppress redundant booking calls during the protected appointment window, but allow a configured appointment-activation or Expedited objective.
4. On completion, trigger disposition-based next steps.
5. On no-show, enter Appointment Recovery using the no-show branch.

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

## WF-07 Path Orchestration

Trigger: a lead event, state change, workflow enrollment, or pending human connection.

1. Read the latest Journey phase, milestone, path tier, appointment, ownership, and conversion state.
2. Validate all required and conditional milestone rules.
3. Select the strongest valid objective.
4. Maintain exactly one active outbound call objective.
5. Route ordinary progress through Standard, additional help through Assisted, valid jumps through Expedited, and failed transitions through Recovery.
6. Before execution or an agent bridge, recheck the state and replace obsolete work.
7. After advancement, suppress superseded calls, tasks, workflows, reminders, and appointments.
8. Record the prior state, new state, path movement, reason, and owner.

## WF-08 Conversion Recovery

Trigger: completed sales conversation without commitment.

1. Capture objection, decision status, next action, and owner.
2. Keep the opportunity inside the configured active sales window.
3. Create an appointment for exact-time commitments, an Assigned Task for personal work, or a Call Queue entry for pooled follow-up.
4. Exit on conversion, disqualification, DND, or transition to reactivation.

## WF-09 Payment Recovery

Trigger: payment initiated but incomplete, declined, abandoned, or overdue.

1. Confirm the customer still intends to proceed.
2. Protect sensitive payment information.
3. Assign the correct owner and due time.
4. Resume onboarding after successful payment.
5. Escalate unresolved discrepancies according to client configuration.

## WF-10 Onboarding Recovery

Trigger: committed customer has incomplete documents, setup, registration, or activation.

1. Identify the missing onboarding requirement.
2. Assign the responsible coordinator.
3. Communicate the exact next step and deadline.
4. Preserve the sales-to-onboarding handoff context.
5. Exit when activation is complete or escalation is accepted.

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
- latest Journey state confirmed;
- exactly one active outbound call objective;
- required milestones and Expedited authority validated.
