# Salesflow Booking Engine

The **Salesflow Booking Engine** is the universal operating framework for service businesses that moves customer interest through **Campaign → Capture → Convert → Close**, then hands the customer to onboarding and support.

The framework has four connected layers:

1. **Customer Journey** — where the customer should go.
2. **Roles and Handoffs** — who owns each transition.
3. **Work Priorities** — what users work on next.
4. **Recoveries** — what happens when a required transition fails.

The Customer Journey uses four operating tiers:

1. **Standard Path** — follow the client's configured journey.
2. **Assisted Path** — provide additional help to complete the expected transition.
3. **Expedited Path** — advance a ready lead beyond one or more expected steps.
4. **Recovery Path** — restore progress after a transition fails, stalls, or becomes invalid.

Its invariant operating order is:

1. **Appointments** — honor scheduled commitments.
2. **Live Calls** — answer inbound calls, warm transfers, and Zero Friction connections.
3. **Assigned Tasks** — complete due and overdue personal responsibilities.
4. **Call Queue** — continuously work pooled follow-up when higher-priority work is clear.

The industries, scripts, pipelines, and service-level targets may change. The work methodology does not.

## Start here

- [Booking Engine operating framework](framework/booking-engine.md)
- [Customer Journey and Path Tiers](framework/customer-journey.md)
- [Roles and ownership](framework/roles-and-ownership.md)
- [Handoffs](framework/handoffs.md)
- [Recovery system](recoveries/README.md)
- [Framework overview](docs/00-start-here.md)
- [The Four Work Priorities](docs/01-work-priorities.md)
- [Appointments](docs/02-appointments.md)
- [Live Calls and Zero Friction](docs/03-live-calls.md)
- [Assigned Tasks](docs/04-assigned-tasks.md)
- [Call Queue](docs/05-call-queue.md)
- [Universal call taxonomy](docs/06-call-types.md)
- [Dispositions and documentation](docs/07-dispositions-documentation.md)
- [Management system and KPIs](docs/08-management-system.md)
- [Salesflow implementation](implementation/salesflow/README.md)
- [Workflow specifications](implementation/salesflow/workflow-specifications.md)
- [Client configuration template](templates/client-profile.yaml)
- [AI maintenance rules](governance/AI-MAINTENANCE.md)

## Core operating loop

When a user logs in:

1. Prepare for and complete appointments due now.
2. Accept live calls when available.
3. Complete assigned tasks that are due or overdue.
4. Work the next eligible Call Queue record.
5. Pause lower-priority work when higher-priority work becomes active.

If the Call Queue falls below capacity, the campaign manager—not the agent—owns restoring eligible work.

## Delivery targets

The content is written in Markdown so it can be delivered through:

- a Salesflow knowledge center;
- a Salesflow custom menu page;
- a Salesflow course or membership product;
- a static documentation site;
- an AI assistant grounded on the repository;
- exported PDFs or onboarding materials.

## Status

Version `0.3.0` establishes the universal four-phase service-business journey and four path tiers. Client-specific implementations should configure milestones, authority, and required steps without rewriting the core rules.
