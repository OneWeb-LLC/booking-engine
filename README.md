# Salesflow Booking Engine

The **Salesflow Booking Engine** is the universal operating framework for service businesses that begins when a lead is submitted and moves that lead through **Capture → booked appointment**. Its objective is to create a valid sales appointment and hand responsibility to the client's closing team.

Salesflow can also support the upstream **Campaign** phase through its ad manager and campaign tools. When the client chooses that service, Salesflow supports **Campaign → Capture → Convert**; when the client supplies its own leads, the Booking Engine operates across **Capture → Convert**. **Close remains the client's responsibility.**

The framework has four connected operating layers:

1. **Customer Journey** — where the customer should go.
2. **Roles and Handoffs** — who owns each transition.
3. **Work Priorities** — what users work on next.
4. **Recoveries** — what happens when a required transition fails.

The Customer Journey uses three operating paths:

1. **Standard Path** — follow the client's configured journey through automation and normal human effort.
2. **Expedited Path** — skip one or more normally expected, skippable steps and advance to a later valid step.
3. **Recovery Path** — restore progress after a transition fails, stalls, or becomes invalid.

Its four canonical work types are listed in priority order:

1. **Appointments** — honor scheduled commitments.
2. **Live Calls** — answer inbound calls, warm transfers, and Zero Friction connections.
3. **Assigned Tasks** — complete due and overdue personal responsibilities.
4. **Call Queue** — continuously work pooled follow-up when higher-priority work is clear.

Not every role owns every work type. Each role page lists its assigned subset and the specific expected work underneath it. The industries, scripts, pipelines, and service-level targets may change. The work methodology does not.

## Living wiki hierarchy

1. **[Methodology](methodology/README.md)** — why the Booking Engine works and the universal rules.
2. **[Roles](roles/README.md)** — who owns each responsibility and the role's authority.
3. **[Salesflow Instructions](salesflow/README.md)** — the complete, click-by-click procedure for performing the work.
4. **[Recoveries](recoveries/README.md)** — how failed or stalled customer transitions are restored.
5. **[Training](training/course-outline.md)** — how employees learn and certify.
6. **[Administration](salesflow/administration/README.md)** — how Salesflow is configured and maintained.
7. **[Snapshot](snapshot/README.md)** — the reserved specification for the future installable configuration.
8. **[Governance](governance/AI-MAINTENANCE.md)** — how the living wiki remains trustworthy.

Employees begin with their role and follow one direct link to the relevant Salesflow instruction. Each instruction combines the operating standard with a Staff Notebook-style walkthrough: where to go, what to click, what to enter, what to verify, and what happens next.

## Core operating loop

When a user logs in:

1. Load the work types assigned to the user's role.
2. Begin the highest-priority assigned type.
3. Complete active customer work before accepting new work.
4. Move to the next assigned type when higher-priority work is clear.
5. Never enter a work area that is not assigned to the role.

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

Version `0.9.0` simplifies the living wiki into a role-first operating system, makes Salesflow procedures the single employee source of truth, reserves Snapshot documentation until the actual Snapshot can be audited, and requires a booked appointment when a warm transfer fails.
