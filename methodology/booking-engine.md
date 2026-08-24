# Salesflow Booking Engine Operating Framework

## Definition

The Salesflow Booking Engine is the coordinated system that begins when a lead is submitted and converts that lead into a valid sales appointment.

It combines communication, automation, people, appointments, tasks, pipelines, reporting, and recovery workflows to move the lead through Capture and the appointment-producing portion of Convert. The Booking Engine ends when the appointment is validly booked and responsibility is handed to the client's closing team.

Salesflow may also create and manage the upstream Campaign phase through its ad manager and campaign services. That makes Salesflow capable of supporting Campaign, Capture, and Convert, but Campaign remains an optional upstream service rather than part of the Booking Engine's core boundary. Close remains the client's responsibility.

## Four-layer architecture

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

Appointments remain the highest scheduled obligation. Inside an active interaction, the user should not schedule an unnecessary future conversation when the customer can responsibly advance now.

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
