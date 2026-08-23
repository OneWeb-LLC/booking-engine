# AI Maintenance Rules

AI may propose, draft, compare, and update this framework, but must preserve the operating contract.

## Invariants

The framework must preserve:

1. the universal Campaign → Capture → Convert → Close journey and four path tiers;
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
7. Keep external vendor sources inside the maintainer reference ledger; employee pages must contain complete Salesflow-branded instructions.
8. Re-verify visible clicks inside Salesflow and update screenshots whenever the interface changes.

## AI review checklist

- Does the change preserve the four priorities?
- Does the change preserve Standard, Assisted, Expedited, and Recovery as the four path tiers?
- Does the change identify the Customer Journey stage and owner?
- Does it distinguish fixed phases from configurable client milestones?
- Does any Expedited movement validate required steps and role authority?
- Does every broken transition have a recovery path?
- Is the Booking Agent preserved as the front-line Booking Engine operator?
- Are purpose, trigger, priority, execution method, and outcome kept separate?
- Could it create duplicate or conflicting calls?
- Does it recheck state and suppress work made obsolete by advancement?
- Are DND, consent, calling hours, and sensitive-data rules preserved?
- Does every workflow have entry, retry, failure, exit, and escalation paths?
- Does the agent know exactly what to do?
- Can management identify whether a failure belongs to the agent, campaign, staffing, or system?
- Does every employee instruction contain its outcome, exact navigation, click-by-click walkthrough, completion, automation, exception, and verification state?
- Does the employee page avoid sending users to an external vendor for instructions?
- Does the change preserve the Methodology → Roles → Salesflow Instructions → Snapshot boundary?

## Versioning

- Patch: clarifications and corrections.
- Minor: backward-compatible capability or workflow additions.
- Major: changes to the core operating contract.
