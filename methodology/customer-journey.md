# Customer Journey and Path Tiers

## Universal journey

The broader Salesflow customer journey for service businesses uses four fixed phases:

1. **Campaign** — generate qualified demand.
2. **Capture** — identify and record the lead, source, consent, and intent.
3. **Convert** — create a qualified sales opportunity through contact, qualification, booking, handoffs, and appointments.
4. **Close** — secure commitment, complete the configured commercial action, and initiate onboarding.

## Booking Engine boundary

The Booking Engine begins when a lead is submitted into Salesflow and the Capture phase starts. Its terminal objective is a valid booked appointment inside Convert. At that point, responsibility transfers to the client's Sales Officer or closing team.

The client is responsible for closing the lead. Salesflow may support the upstream Campaign phase through its ad manager and campaign services when the client chooses that service. Therefore:

- **Booking Engine core:** Capture → booked appointment within Convert;
- **Salesflow with client-supplied leads:** Capture + Convert;
- **Salesflow with campaign management:** Campaign + Capture + Convert;
- **Client closing team:** the remaining Convert activity, when applicable, and Close.

## Configurable journey depth

The phases remain universal; milestones inside them are configurable. Most service-business variation belongs inside Convert. The Booking Engine's configured milestones end at the booked-appointment milestone; later sales milestones belong to the client's closing process.

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
| Convert — Booking Engine | Valid booked appointment and accepted handoff to the closing team | Booking Agent | Booking or Appointment Recovery |
| Convert — Client sales process | Conduct the appointment and advance the qualified opportunity | Sales Officer | Client sales follow-up |
| Close | Commitment and configured commercial action completed | Sales Officer | Client conversion or payment process |
