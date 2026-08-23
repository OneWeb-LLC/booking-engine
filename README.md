# Salesflow Work System

The Salesflow Work System is a portable operating framework for keeping customer-facing teams responsive, accountable, and continuously productive.

Its invariant operating order is:

1. **Appointments** — honor scheduled commitments.
2. **Live Calls** — answer inbound calls, warm transfers, and Zero Friction connections.
3. **Assigned Tasks** — complete due and overdue personal responsibilities.
4. **Call Queue** — continuously work pooled follow-up when higher-priority work is clear.

The industries, scripts, pipelines, and service-level targets may change. The work methodology does not.

## Start here

- [Framework overview](docs/00-start-here.md)
- [The Four Work Priorities](docs/01-work-priorities.md)
- [Appointments](docs/02-appointments.md)
- [Live Calls and Zero Friction](docs/03-live-calls.md)
- [Assigned Tasks](docs/04-assigned-tasks.md)
- [Call Queue](docs/05-call-queue.md)
- [Universal call taxonomy](docs/06-call-types.md)
- [Dispositions and documentation](docs/07-dispositions-documentation.md)
- [Management system and KPIs](docs/08-management-system.md)
- [GoHighLevel implementation](implementation/gohighlevel/README.md)
- [Workflow specifications](implementation/gohighlevel/workflow-specifications.md)
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
- a GoHighLevel custom menu page;
- a GoHighLevel course or membership product;
- a static documentation site;
- an AI assistant grounded on the repository;
- exported PDFs or onboarding materials.

## Status

Version `0.1.0` establishes the universal framework. Client-specific implementations should extend the framework through configuration rather than rewriting its core rules.

