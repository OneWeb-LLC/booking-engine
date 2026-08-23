# Call Queue

## Purpose

The Call Queue keeps eligible agents productive after higher-priority work is clear. It is pooled work supplied by campaigns, workflows, recovery logic, and reactivation programs.

## Agent standard

1. Open the Call Queue when no appointment, Live Call, or due Assigned Task requires attention.
2. Accept the next eligible record.
3. Read the Call Brief.
4. Place the call using the approved number and script framework.
5. Select exactly one disposition.
6. Add meaningful notes when context must be preserved.
7. Allow the disposition workflow to determine the next action.

## Required Call Brief

- call purpose;
- trigger;
- priority;
- attempt number;
- last outcome;
- relevant context;
- desired outcome;
- next-action rule.

See `templates/call-brief.md`.

## Queue sources

- new-lead activation recovery;
- missed inbound calls;
- high-intent engagement;
- appointment confirmations;
- no-show recovery;
- booking abandonment;
- active lead follow-up;
- reactivation;
- manually approved campaigns.

## Queue ordering

Queue priority should consider:

1. promised or legally required timing;
2. freshness of intent;
3. due time;
4. call purpose;
5. attempt count;
6. contact eligibility;
7. agent skill and ownership constraints.

## Collision prevention

A contact should generally have only one active outbound call instruction. Before enrollment, check for active appointments, live conversations, owned callbacks, open Manual Actions, DND, terminal outcomes, and duplicate workflows.

## Exit conditions

- connected and progressed;
- booked;
- callback scheduled;
- cadence exhausted;
- disqualified;
- not interested;
- wrong number;
- DND;
- won or otherwise completed.

## Management responsibility

The campaign manager owns queue supply. The system should warn before the queue reaches zero, using estimated productive hours rather than raw contact count.

