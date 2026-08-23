# Salesflow Booking Engine

The **Salesflow Booking Engine** is the universal operating framework for service businesses that moves customer interest through **Campaign → Capture → Convert → Close**, then hands the customer to onboarding and support.

The framework has four connected operating layers:

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

- [Documentation map](docs/README.md)
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

## Documentation layers

The repository separates doctrine from execution:

1. **Framework** — universal rules and decision logic.
2. **Playbooks** — what each role owns and does.
3. **Procedures** — exact Salesflow navigation and clicks.
4. **Implementation** — how administrators configure and maintain the system.

Employees should begin with their role playbook and open a procedure only when they need exact execution steps. Maintainers use the framework, implementation specifications, governance rules, and source ledger.

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

Version `0.4.0` adds the Salesflow-owned documentation and training architecture, universal role playbooks, and frontline click-by-click procedures. Client-specific implementations should configure milestones, authority, scripts, and screenshots without rewriting the core rules.
