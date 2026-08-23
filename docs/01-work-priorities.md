# The Four Work Priorities

## 1. Appointments

Appointments are scheduled commitments. They include meetings, consultations, demos, service appointments, and exact-time callbacks.

Only appointments that are active or inside their preparation window should interrupt other work. A later appointment must not block productive work earlier in the day.

## 2. Live Calls

Live Calls represent a person available now. They include:

- inbound calls;
- warm transfers;
- Zero Friction connections;
- returned calls;
- AI-to-human transfers;
- urgent live escalations.

Live Calls interrupt ordinary assigned tasks and Call Queue work, but never an active appointment or active call.

## 3. Assigned Tasks

Assigned Tasks are due or overdue responsibilities owned by a specific person. Examples include sending a proposal, reviewing documents, resolving an issue, or completing a promised follow-up.

An exact-time callback must be scheduled as an appointment. A pooled call instruction is a Call Brief, not an Assigned Task.

## 4. Call Queue

The Call Queue is the default productive state. When no higher-priority work is active, an eligible agent works the next pooled record.

Agents do not choose favorites from the queue. Routing logic supplies the best eligible record according to priority, due time, attempt count, skill, and ownership rules.

## Interruption rules

| Current work | Higher-priority event | Expected behavior |
|---|---|---|
| Active appointment | Any new work | Do not interrupt; route elsewhere |
| Active call | Any new work | Do not interrupt; route elsewhere |
| Wrap-up | Live Call | Allow short protected wrap-up, then route |
| Assigned Task | Live Call | Pause safely and accept |
| Call Queue | Appointment or Live Call | Pause immediately |
| Call Queue | Assigned Task becomes due | Finish current call, then complete task |

## Availability states

- **Available:** eligible for live routing.
- **In Appointment:** protected from interruptions.
- **On Call:** protected from interruptions.
- **Wrap-Up:** temporarily protected for documentation.
- **Break:** unavailable.
- **Offline:** unavailable.

