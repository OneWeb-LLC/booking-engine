# Customer Journey and Path Tiers

## Universal journey

The Salesflow Booking Engine is built for service businesses and uses four fixed phases:

1. **Campaign** — generate qualified demand.
2. **Capture** — identify and record the lead, source, consent, and intent.
3. **Convert** — create a qualified sales opportunity through contact, qualification, booking, handoffs, and appointments.
4. **Close** — secure commitment, complete the configured commercial action, and initiate onboarding.

The Booking Engine ends with an accepted onboarding handoff. Onboarding and Support continue the broader Customer Journey.

## Configurable journey depth

The phases remain universal; milestones inside them are configurable. Most service-business variation belongs inside Convert.

A simple journey may use one consultation appointment. A longer journey may use discovery, assessment, demonstration, consultation, approval, or multiple appointments before Close.

Each milestone must declare whether it is:

- **required:** may not be skipped;
- **conditional:** required only when its condition applies; or
- **skippable:** may be bypassed when the Expedited rule is satisfied.

## Four path tiers

### Tier 1 — Standard Path

The lead follows the client's configured journey without exceptional intervention. The Standard Path may include automation, Booking Agents, appointments, Sales Officers, payments, and human handoffs. Standard does not mean self-service or human-free.

### Tier 2 — Assisted Path

The lead needs additional help to complete the expected transition. The assistance should return the lead to the configured Standard Path whenever practical.

Examples include answering pre-booking questions, completing missing information, helping select an appointment, and removing an ordinary obstacle.

### Tier 3 — Expedited Path

The lead demonstrates readiness or capability to advance beyond one or more expected funnel steps. Expedited is defined by the valid jump forward—not by a specific method, channel, or role.

Examples include:

- completing a configured Buy Now option;
- requesting an immediate conversation with a Sales Officer;
- accepting a warm transfer instead of booking;
- closing within the Booking Agent's authorized limits;
- converting before an upcoming appointment; or
- legitimately skipping a later Convert milestone.

Expedited movement may emerge from either Standard or Assisted.

### Tier 4 — Recovery Path

A required transition has failed, stalled, or become invalid. The appropriate Recovery restores the lead to the strongest valid next step. Recovery may rejoin Standard, Assisted, or Expedited, or end in a valid exit state.

Recovery is taught as Tier 4 for operating clarity, but architecturally it surrounds the entire journey.

## Advancement rule

Move every lead through the Standard Path by default. Assist when necessary. Expedite when readiness permits. Recover when progress breaks.

Expedited movement must advance to the furthest **valid** stage. It may never bypass applicable consent, legal, compliance, eligibility, payment, safety, or mandatory service requirements.

Whenever a lead changes paths or jumps ahead, Salesflow must recheck the current state, record the reason, assign the new objective, and suppress obsolete calls, tasks, workflows, and appointments.

## Journey matrix

| Phase | Ideal outcome | Default owner | Typical broken transition |
|---|---|---|---|
| Campaign | Qualified demand enters Salesflow | Campaign Manager | Activation Recovery |
| Capture | Valid, consented, attributable lead record | Campaign Manager/System | Activation Recovery |
| Convert | Qualified appointment, live handoff, or sales-ready opportunity | Booking Agent/Sales Officer | Booking or Appointment Recovery |
| Close | Commitment and configured commercial action completed | Sales Officer | Conversion or Payment Recovery |
| Onboarding handoff | Context and responsibility accepted | Onboarding Coordinator | Onboarding Recovery |
