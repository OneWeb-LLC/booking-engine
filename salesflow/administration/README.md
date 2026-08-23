# Salesflow Implementation

## Recommended delivery architecture

Use Salesflow for execution and this version-controlled repository for governance.

- **GitHub:** canonical framework and change history.
- **Salesflow custom page:** daily operating dashboard and quick-reference system.
- **Salesflow course:** structured onboarding, demonstrations, quizzes, and certification.
- **Salesflow workflows:** routing, tasks, Manual Actions, reminders, suppression, and reporting events.

The custom page and course should be generated or updated from this repository where practical. Do not allow independent copies to drift without a version number.

See the [knowledge-center delivery specification](knowledge-center.md) for the employee experience.

## Required Salesflow components

- calendars and appointment types;
- team users and skill groups;
- phone numbers and routing;
- custom fields for active call reason, priority, due time, attempt number, and work owner;
- custom dispositions;
- Manual Action workflows;
- Zero Friction workflow or integration;
- suppression and collision checks;
- recovery and reactivation workflows;
- reporting dashboards.
- Customer Journey stages and ownership;
- four-phase Journey, path-tier, and recovery workflow mappings;
- handoff records with context, owner, and acceptance state.

## Native versus Snapshot boundary

| Capability | Native Salesflow source | Snapshot responsibility |
|---|---|---|
| Contacts and identity | Contact record | Required field mapping and quality rules |
| Appointments | Calendars and appointment statuses | Milestone mapping, views, reminders, and Recovery orchestration |
| Personal work | Assigned Tasks | Role rules, views, escalation, and workflow creation |
| Pooled calls | Manual Actions | Queue supply, Call Brief, objective locking, retries, and suppression |
| Calls | Dialer, routing, and transfers | Zero Friction objectives, skill routing, and failure behavior |
| Call outcomes | Dispositions | Canonical labels, workflow mapping, and reporting categories |
| Lifecycle | Opportunities, pipelines, stages, and statuses | Campaign → Capture → Convert → Close mapping and path fields |
| Knowledge | Custom menu and course capabilities | Booking Engine workspace, role access, wiki, and certification |

The installed component catalog belongs in the [Booking Engine Snapshot](../../snapshot/README.md). Do not describe a planned custom component as native Salesflow behavior.

## Recommended custom menu

1. My Appointments
2. Live Calls
3. My Assigned Tasks
4. Call Queue
5. Scripts and Knowledge
6. My Performance

## Course recommendation

Use a short certification course for initial training:

1. The Four Work Priorities
2. Appointments
3. Inbound and Zero Friction
4. Assigned Tasks
5. Call Queue and Call Briefs
6. Dispositions and Documentation
7. Client-specific scripts and compliance
8. Journey Phases, Path Tiers, and Recoveries
9. Roles and Handoffs
10. Practical assessment

The course teaches and certifies the system. The custom page operates the system. Both must link to the same versioned Roles, Actions, and Salesflow Instructions.
