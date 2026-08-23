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

## Living wiki hierarchy

1. **[Methodology](methodology/README.md)** — why the Booking Engine works and the universal rules.
2. **[Roles](roles/README.md)** — who owns each responsibility and the role's authority.
3. **[Actions](actions/README.md)** — what outcome must be accomplished, independent of software.
4. **[Salesflow Instructions](salesflow/README.md)** — how to execute the action in Salesflow.
5. **[Snapshot](snapshot/README.md)** — what custom configuration, fields, workflows, and navigation are installed.
6. **[Training](training/course-outline.md)** — how employees learn and certify.
7. **[Governance](governance/AI-MAINTENANCE.md)** — how the living wiki remains trustworthy.

Employees begin with their role. Each responsibility links to a reusable action standard and the exact Salesflow instruction. Native instructions are separated from Snapshot-dependent instructions.

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

Version `0.5.0` establishes the living-wiki hierarchy, separates methodology from product instructions, and creates the versioned Snapshot namespace for native mappings, custom fields, workflows, pipelines, calendars, routing, dispositions, navigation, and dashboards.
