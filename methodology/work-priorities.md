# Work Priorities

The universal employee operating order is:

1. **Appointments** — honor active scheduled commitments.
2. **Live Calls** — serve people available now.
3. **Assigned Tasks** — complete due personal responsibilities.
4. **Call Queue** — work the next eligible pooled record.

Only active work or an appointment inside its preparation window interrupts lower-priority work. An active appointment or call is never interrupted by new work.

Work Priority determines what the user handles next. The Journey Advancement Rule determines how far the active customer should move: continue Standard, Assist when necessary, Expedite when readiness permits, or enter Recovery.

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
