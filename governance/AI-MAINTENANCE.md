# AI Maintenance Rules

AI may propose, draft, compare, and update this framework, but must preserve the operating contract.

## Invariants

The framework must preserve:

1. the Customer Journey and Golden Path;
2. functional roles and explicit handoffs;
3. the Four Work Priorities: Appointments, Live Calls, Assigned Tasks, Call Queue;
4. named recovery paths for broken journey transitions.

The invariant may be changed only by an explicit governance decision, not as a side effect of a client customization.

## Change procedure

1. Identify whether the change is universal or client-specific.
2. Prefer configuration for client-specific differences.
3. State which workflows, pages, training lessons, reports, and templates are affected.
4. Check for contradictions and duplicate instructions.
5. Update the framework version and changelog.
6. Require human review before deployment into client accounts.

## AI review checklist

- Does the change preserve the four priorities?
- Does the change identify the Customer Journey stage and owner?
- Does every broken transition have a recovery path?
- Is the Booking Agent preserved as the front-line Booking Engine operator?
- Are purpose, trigger, priority, execution method, and outcome kept separate?
- Could it create duplicate or conflicting calls?
- Are DND, consent, calling hours, and sensitive-data rules preserved?
- Does every workflow have entry, retry, failure, exit, and escalation paths?
- Does the agent know exactly what to do?
- Can management identify whether a failure belongs to the agent, campaign, staffing, or system?

## Versioning

- Patch: clarifications and corrections.
- Minor: backward-compatible capability or workflow additions.
- Major: changes to the core operating contract.
