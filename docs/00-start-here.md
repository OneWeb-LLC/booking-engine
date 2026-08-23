# Start Here: The Booking Engine Work System

## Purpose

This framework governs the complete Customer Journey through the Salesflow Booking Engine. It defines what should happen when conversion proceeds ideally, who owns each step, what users should work on next, and how to recover when progress breaks.

The Booking Engine is not merely a calendar or call workflow. It is the coordinated system that moves a person from interest to activation and ongoing support.

Every user works from the same priority system while Salesflow supplies, routes, and protects the work.

## Framework model

- **Golden Path:** the ideal conversion journey.
- **Roles:** functional ownership across that journey.
- **Handoffs:** the transfer of context and responsibility.
- **Work Priorities:** the daily execution order.
- **Recoveries:** named exception paths when the Golden Path breaks.

## The operating promise

The system must ensure that:

- scheduled commitments are honored;
- live demand receives an immediate response;
- delegated responsibilities do not disappear;
- pooled follow-up keeps available agents productive;
- every interaction produces a valid outcome and next system action;
- no contact receives conflicting calls from multiple workflows;
- management can see both execution and work supply.

## Universal roles

Role names may be changed by each client, but the responsibilities remain.

### Agent

- Maintains accurate availability.
- Handles appointments and live calls.
- Completes assigned work.
- Works the Call Queue when available.
- Records dispositions and meaningful context.

### Booking Agent

- Operates the front end of the Booking Engine.
- Activates, qualifies, books, routes, and protects live momentum.
- Recovers missed calls, failed connections, and incomplete bookings.

### Sales Representative

- Conducts qualified sales conversations.
- Handles objections and advances commitment.
- Owns conversion and active sales follow-up.

### Onboarding Coordinator

- Completes payment, paperwork, activation, and the post-sale handoff.

### Support Representative

- Resolves post-conversion needs and protects the customer relationship.

### Campaign Manager

- Maintains lead and queue supply.
- Owns workflow enrollment, cadence, and suppression.
- Monitors queue depth, response times, and conversion.
- Corrects automation or campaign failures.

### Team Manager

- Owns staffing, coaching, schedule coverage, and quality.
- Resolves overdue commitments and escalations.
- Reviews outcomes rather than activity alone.

### System Administrator

- Maintains permissions, integrations, calendars, phone numbers, fields, and workflow integrity.

## Client-specific configuration

Do not hard-code industry language into the universal framework. Each implementation should define:

- role names;
- appointment types;
- business hours and time zone;
- preparation windows;
- service-level targets;
- call attempts and cadence;
- pipeline stages;
- dispositions;
- skill groups;
- escalation paths;
- suppression and compliance requirements.

Use `templates/client-profile.yaml` as the configuration contract.
