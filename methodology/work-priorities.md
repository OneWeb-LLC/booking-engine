# Work Priorities

The Booking Engine uses four canonical work types in priority order:

1. **Appointments** — honor active scheduled commitments.
2. **Live Calls** — serve people available now.
3. **Assigned Tasks** — complete due personal responsibilities.
4. **Call Queue** — work the next eligible pooled record.

These work types remain canonical across Salesflow, but a role only receives the types assigned to it. The role page defines the specific calls, appointments, tasks, and queued work expected within each type.

The priority order applies only among work types assigned to that user. Only active work or an appointment inside its preparation window interrupts lower-priority work. An active appointment or call is never interrupted by new work.

Work Priority determines what the user handles next. The Journey Advancement Rule determines how far the active customer should move: continue Standard, Expedite when a step can be validly skipped, or enter Recovery.

## Interruption rules

| Current work | Higher-priority event | Expected behavior |
|---|---|---|
| Active appointment | Any new work | Do not interrupt; route elsewhere |
| Active call | Any new work | Do not interrupt; route elsewhere |
| Wrap-up | Live Call | Allow short protected wrap-up, then route |
| Assigned Task | Live Call | Pause safely and accept |
| Call Queue | Appointment or Live Call | Pause immediately |
| Call Queue | Assigned Task becomes due | Finish the current call, then complete the task |

## Availability states

- **Available:** eligible for live routing.
- **In Appointment:** protected from interruptions.
- **On Call:** protected from interruptions.
- **Wrap-Up:** temporarily protected for documentation.
- **Break:** unavailable.
- **Offline:** unavailable.

## Role-to-work-type matrix

| Role | Assigned work types | Expected work underneath |
|---|---|---|
| Booking Agent | Live Calls → Assigned Tasks → Call Queue | Inbound sales, admissions, general-business and initial support calls; Zero Friction connections; personally owned follow-up; pooled Lead Activation, missed-call, booking-recovery and reactivation calls |
| Sales Officer | Appointments → Live Calls → Assigned Tasks | Scheduled sales appointments; warm transfers initiated by Booking Agents; personally owned sales follow-up |
| Onboarding Coordinator | Appointments → Live Calls → Assigned Tasks | Scheduled onboarding commitments; accepted live onboarding handoffs; personally owned onboarding requirements |
| Support Officer | Live Calls → Assigned Tasks → Call Queue | Routed or transferred support calls; owned resolutions and escalations; pooled support follow-up when configured |
| Campaign Manager | Assigned Tasks | Campaign, workflow, attribution, suppression and queue-supply work |
| Team Manager | Live Calls → Assigned Tasks | Accepted escalations, coverage intervention, QA and coaching work |
| Salesflow Administrator | Assigned Tasks | Configuration, verification, incident and change-control work |

A role may receive an additional work type only when the client profile explicitly enables it. Combining roles combines their assigned work types; it does not change the canonical definitions.
