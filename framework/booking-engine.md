# Salesflow Booking Engine Operating Framework

## Definition

The Salesflow Booking Engine is the coordinated system that converts customer interest into a committed, onboarded, and supported customer.

It combines campaigns, communication, automation, people, appointments, tasks, pipelines, payments, onboarding, reporting, and recovery workflows into one controlled Customer Journey.

## Four-layer architecture

### 1. Customer Journey

Defines the universal phases—Campaign, Capture, Convert, and Close—the client's configured milestones, and the strongest valid next destination.

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

## Four path tiers

1. **Standard Path:** the lead follows the client's configured journey without exceptional intervention.
2. **Assisted Path:** the team provides additional help to complete the expected transition.
3. **Expedited Path:** readiness or capability allows the lead to advance beyond one or more expected steps.
4. **Recovery Path:** Salesflow and the team restore progress after a transition fails, stalls, or becomes invalid.

The tiers classify how a customer is moving; they are not a best-to-worst score. Expedited may emerge from Standard or Assisted. Recovery surrounds the whole journey and returns the customer to the strongest valid path.

## Two decision systems

The **Work Priority** tells a user what to handle next: Appointments → Live Calls → Assigned Tasks → Call Queue.

The **Advancement Rule** tells the user how far to move the customer already being handled: continue Standard, provide Assistance, Expedite to the furthest valid stage, or enter Recovery.

Appointments remain the highest scheduled obligation. Inside an active interaction, the user should not schedule an unnecessary future conversation when the customer can responsibly advance now.

## Operating principles

- Preserve live momentum.
- Honor scheduled commitments.
- Use the Standard Path by default.
- Assist when necessary.
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
