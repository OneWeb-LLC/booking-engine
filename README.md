# Salesflow Booking Engine

The **Salesflow Booking Engine** is the universal revenue operating framework for service businesses. It understands and coordinates the full lifecycle **Campaign → Capture → Convert → Close**, even when a specific client deploys only part of that lifecycle. Its purpose is to ensure that demand does not die between marketing, lead capture, contact, booking, show, close, payment, and handoff.

The system is defined through two dimensions: the **customer lifecycle** (Campaign, Capture, Convert, Close) and the **implementation stack** (Strategy & Measurement, Software, Hardware & Channels, Human Execution). This prevents the Booking Engine from being reduced to a calendar or automation package and makes the required operating system explicit.

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

During a Booking Call, a ready lead is closed immediately when the Booking Agent is authorized; otherwise the agent initiates a warm transfer, with a booked appointment as the protected fallback. Not every role owns every work type. Each role page lists its assigned subset and the specific expected work underneath it. The industries, scripts, pipelines, and service-level targets may change. The work methodology does not.

## Living wiki hierarchy

1. **[Methodology](methodology/README.md)** — the universal Booking Engine doctrine, including the [Revenue System Architecture](methodology/revenue-system-doctrine.md).
2. **[Customer Journey](customer-journey/README.md)** — phases, milestones, boundaries, and operating paths.
3. **[Roles](roles/README.md)** — core, receiving, and downstream ownership plus employee procedures and training.
4. **[Work Priorities](work-priorities/README.md)** — canonical work types, role assignment, call types, callbacks, and interruption rules.
5. **[Snapshot](snapshot/README.md)** — installable configuration, administration, templates, verification, change control, and explicitly marked pilots/reference architecture.
6. **[Governance](governance/README.md)** — documentation integrity, source maintenance, and architecture.
7. **[Pilots](pilots/three-company-masterplan.md)** — phased real-world deployment across Gabriel Health Institute, Montessori Bilingual Academy, and Eola Masonic Lodge.

Employees begin with their role and follow one direct link to the relevant Salesflow instruction. Each instruction combines the operating standard with a Staff Notebook-style walkthrough: where to go, what to click, what to enter, what to verify, and what happens next.

## Core operating loop

When a user logs in:

1. Load the work types assigned to the user's role.
2. Begin the highest-priority assigned type.
3. Complete active customer work before accepting new work.
4. Move to the next assigned type when higher-priority work is clear.
5. Never enter a work area that is not assigned to the role.

If the Call Queue falls below capacity, the campaign manager—not the agent—owns restoring eligible work.

## Communications pilot

The current GHI reference experiment is documented in [Snapshot → Communications Workstation Pilot](snapshot/communications-pilot.md).

It tests:

- **Yealink WH63 E2 UC** as the on-site headset standard;
- **MicroSIP** as the first Windows SIP softphone candidate against HighLevel/Twilio SIP credentials;
- headset-button answer/end without keyboard or mouse dependency;
- physical **Yealink T34W** endpoints only where computer-off continuity is actually required;
- future presence-aware paging/push-to-talk;
- spoken appointment reminders through the headset, currently nicknamed **Remindly**.

This is deliberately marked as a pilot. It must preserve Salesflow call logging, recordings, automation, attribution and customer-record integrity before it can become a supported Snapshot component.

## Delivery targets

The content is written in Markdown so it can be delivered through:

- a Salesflow knowledge center;
- a Salesflow custom menu page;
- a Salesflow course or membership product;
- a static documentation site;
- an AI assistant grounded on the repository;
- exported PDFs or onboarding materials.

## Status

Version `0.10.0` simplifies the living wiki into a role-first operating system, makes Salesflow procedures the single employee source of truth, reserves Snapshot documentation until the actual Snapshot can be audited, and requires a booked appointment when a warm transfer fails.

Current communications work is intentionally stored as **pilot/reference architecture**, not as an already-installed universal Snapshot feature.
