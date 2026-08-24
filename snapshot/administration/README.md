# Salesflow Implementation

## Recommended delivery architecture

Use Salesflow for execution and this version-controlled repository for governance.

- **GitHub:** canonical framework and change history.
- **Salesflow custom page:** daily operating dashboard and quick-reference system.
- **Salesflow course:** structured onboarding, demonstrations, quizzes, and certification.
- **Salesflow workflows:** routing, tasks, Manual Actions, reminders, suppression, and reporting events.

The custom page and course should be generated or updated from this repository where practical. Do not allow independent copies to drift without a version number.

See the [knowledge-center delivery specification](knowledge-center.md) for the employee experience.

## Implementation discovery checklist

Before deploying the framework, audit the target account for:

- calendars, appointment types, users, permissions, and availability;
- phone numbers, inbound routing, transfers, recording, and calling permissions;
- tasks, Manual Actions, opportunities, pipelines, stages, statuses, and dispositions;
- Zero Friction entry, connection, failure, and suppression behavior;
- Recovery and reactivation behavior;
- client scripts, compliance rules, escalation contacts, and reporting requirements.

Use core Salesflow capabilities wherever they satisfy the operating requirement. Do not create custom fields, workflows, dispositions, or navigation merely because an earlier draft proposed them.

The actual installable component catalog will belong in the [Booking Engine Snapshot](../README.md) after the final Snapshot is built and audited. Until then, the Snapshot section remains intentionally blank.

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

The course teaches and certifies the system. The custom page operates the system. Both must link to the same versioned Roles and Salesflow Instructions.
