# Booking Engine Methodology

## Definition

The Salesflow Booking Engine is the coordinated revenue system that turns attention into a completed commercial outcome. It understands the full lifecycle **Campaign → Capture → Convert → Close** and can be deployed across all or part of that lifecycle depending on client scope.

It combines strategy, measurement, software, hardware/channels, automation, people, appointments, tasks, communications, reporting, training, closing, and recovery workflows. The system is intentionally broader than scheduling: a booking is one conversion milestone inside a complete revenue journey.

## Revenue system architecture

See [Revenue System Doctrine](revenue-system-doctrine.md) for the full 4×4 model: **Campaign / Capture / Convert / Close × Strategy & Measurement / Software / Hardware & Channels / Human Execution**.

The operating methodology below remains the execution framework used inside that broader revenue system.

## Four operating layers

### 1. Customer Journey

Defines the broader phases—Campaign, Capture, Convert, and Close—while the Booking Engine specifically owns Capture through the booked-appointment milestone inside Convert.

### 2. Roles and Handoffs

Defines who owns each stage, what authority they have, and how responsibility transfers.

### 3. Work Priorities

Defines the user's daily operating order:

1. Appointments
2. Live Calls
3. Assigned Tasks
4. Call Queue

### 4. Recoveries

Defines what Salesflow and the team do when a required transition does not progress.

## Three operating paths

1. **Standard Path:** the lead follows the client's configured journey through the normal combination of automation and human effort.
2. **Expedited Path:** the lead skips one or more normally expected, skippable steps and advances to a later valid step.
3. **Recovery Path:** Salesflow and the team restore progress after a transition fails, stalls, or becomes invalid.

The paths classify how a customer is moving; they are not a best-to-worst score. Expedited is defined by a valid skipped step, not by speed or human involvement. Recovery surrounds the journey and returns the customer to the strongest valid path.

## Two decision systems

The **Work Priority** tells a user what to handle next: Appointments → Live Calls → Assigned Tasks → Call Queue.

The **Advancement Rule** tells the user how far to move the customer already being handled: continue Standard, Expedite to the furthest valid stage when a step can be validly skipped, or enter Recovery.

Appointments remain the highest scheduled obligation. Inside an active Booking Call, the agent should not schedule an unnecessary future appointment when the customer can responsibly advance now. Close immediately when the Booking Agent is authorized. If the agent is not authorized, initiate a warm transfer to an authorized Sales Officer. Use the correct appointment as the protected fallback when an immediate close or accepted transfer is unavailable.

## Operating principles

- Preserve live momentum.
- Honor scheduled commitments.
- Use the Standard Path by default.
- Expedite when readiness permits.
- Recover when progress breaks.
- Never leave ownership ambiguous.
- Use the correct Salesflow object for the work.
- Every interaction must create clarity.
- Every broken transition must enter a named recovery.
- Activity is not success; customer movement is success.

## Generic by configuration

The framework uses universal functional roles and phases. Clients may add, repeat, or rename milestones without changing the universal journey. For example, the Convert phase may contain one appointment or a sequence of discovery and consultation appointments.

Clients may also change display names without changing responsibilities. For example, a Sales Officer may be called an Admissions Officer, Comfort Advisor, Account Executive, or Enrollment Advisor.

Booking Agent remains a universal role because it is native to the Booking Engine methodology.

## Methodology sections

- [Customer Journey](../customer-journey/README.md)
- [Operating Paths](../customer-journey/README.md#three-operating-paths)
- [Work Priorities](../work-priorities/README.md)
- [Call Types](../work-priorities/call-types.md)
- [Roles](../roles/README.md)
- [Handoffs](handoffs.md)
- [Recoveries](recoveries/README.md)
- [Snapshot](../snapshot/README.md)
- [Governance](../governance/WIKI-ARCHITECTURE.md)


## Real-world validation

The doctrine is being validated through the [Three-Company Revenue Engine Pilot Masterplan](../pilots/three-company-masterplan.md). Repeated needs discovered across the pilots should be promoted into core or configurable platform capabilities according to the productization rule in the doctrine.
