# Booking Engine Doctrine — Revenue System Architecture

## Definition

A Booking Engine is not a calendar or a collection of automations. It is the coordinated revenue system that turns attention into a completed commercial outcome.

The universal lifecycle is:

**Campaign → Capture → Convert → Close**

The Booking Engine may be deployed with only part of the lifecycle when a client already owns upstream or downstream functions, but the doctrine must understand the entire chain because leakage in any stage can destroy the value created elsewhere.

## The two-dimensional model

Every implementation is designed across two dimensions.

### Lifecycle
1. **Campaign** — create qualified demand.
2. **Capture** — identify, record, route, and activate the lead.
3. **Convert** — contact, qualify, book, nurture, recover, and get the prospect to the sales event.
4. **Close** — secure commitment, payment/enrollment/membership, and clean handoff into fulfillment.

### Implementation Stack
1. **Strategy & Measurement** — offer, audience, journey, standards, KPIs, attribution, escalation rules.
2. **Software** — CRM, automations, forms, landing pages, calendars, communications, AI, dashboards, ticketing.
3. **Hardware & Channels** — phones, headsets, workstations, SMS, email, web chat, video, physical endpoints.
4. **Human Execution** — ownership, scripts, SOPs, live calls, training, coaching, QA, escalation, accountability.

The lifecycle tells us **where the customer is**.
The implementation stack tells us **what must exist to move them forward**.

## 4×4 doctrine matrix

| Lifecycle | Strategy & Measurement | Software | Hardware & Channels | Human Execution |
|---|---|---|---|---|
| Campaign | ICP, offer, budget, channel strategy, CPL targets, attribution | Ad manager, campaign tracking, landing-page builder, analytics | Creative capture tools, cameras/mics when needed | Campaign manager, creative production, campaign review |
| Capture | Lead fields, consent, routing rules, response SLA, source tracking | Landing pages, forms, CRM, attribution, dedupe, routing, notifications | SMS, email, phone endpoints, push alerts | Lead ownership, immediate response, data verification |
| Convert | Qualification logic, booking rules, follow-up cadence, show-rate strategy, recovery rules | Calendars, workflows, task queues, video accelerators, chatbot, call logging, next-best-action, nurture, no-show recovery | SIP phones, headsets, softphones, SMS, email, video delivery, chat | Booking agents, scripts, objection handling, warm transfers, appointment confirmation, coaching |
| Close | Sales process, authority limits, pricing/payment rules, close-rate targets, lost-reason taxonomy | Pipeline, proposals, checkout/payment, e-sign, enrollment, dispositioning, revenue attribution | Phone/video meeting endpoints, terminals where applicable | Sales officer/admissions/enrollment staff, closing script, payment collection, handoff |

## Required system components

A mature Booking Engine should account for the following components, even when a specific client does not need every one.

### Campaign
- Offer and audience definition
- Campaign plan
- Paid/organic traffic sources
- Creative assets
- Landing pages
- Attribution and source tracking
- Campaign KPI dashboard

### Capture
- Forms and lead intake
- Consent
- CRM record creation
- Source/campaign attribution
- Language/territory/skill routing
- Immediate staff notification
- Lead response timer
- Duplicate handling
- Lead ownership

### Convert
- Phone system
- SIP/softphone/deskphone configuration
- Professional headsets
- SMS and email
- Zero Friction lead activation
- Call queue
- Tasks
- Calendar and booking logic
- Warm transfers
- Video Accelerators at conversion gates
- Appointment confirmations
- Reminder sequences
- No-show recovery
- Long-term nurture
- AI chatbot / AI assistant
- Staff assist / next-best-action
- Knowledge base and contextual training
- Support/ticket escalation
- Call logging and recordings

### Close
- Sales/admissions playbook
- Offer presentation
- Objection handling
- Payment or enrollment workflow
- Checkout / terminal / payment link where applicable
- Lost-reason capture
- Revenue attribution
- Customer handoff
- Reactivation for undecided prospects

## Journey state model

Each lead must have one authoritative journey state. Example universal states:

`NEW_LEAD`
→ `CONTACTING`
→ `CONTACTED`
→ `QUALIFIED`
→ `BOOKED`
→ `CONFIRMED`
→ `SHOWED`
→ `CLOSED_WON`

Recovery / branch states may include:

- `NO_RESPONSE`
- `NEEDS_FOLLOWUP`
- `NO_SHOW`
- `LOST`
- `SUPPORT_BLOCKED`
- `DISQUALIFIED`

A state transition must trigger the correct automations, assignments, suppression rules, reporting, and next-best action.

## Video Accelerators

Video is treated as a conversion component, not generic marketing content.

Recommended gates:
1. Lead submitted
2. Before booking
3. Immediately after booking
4. Before appointment
5. After no-show
6. Before commitment/payment
7. Immediately after close

Every video must have a single job: move the prospect to the next valid stage.

## Human operating doctrine

The system should reduce unnecessary dependence on memory, awareness, and improvisation.

If a competent employee repeatedly misses an outcome, first inspect:
- notification failure,
- unclear ownership,
- missing training,
- poor tools,
- ambiguous next action,
- unrealistic SLA,
- broken handoff,
- missing recovery.

Human execution remains essential, but the company must make the correct action obvious and easy.

## Training doctrine

Every revenue role should have:
- written SOP,
- short video training,
- example call or demonstration,
- contextual help at the moment of work,
- recurring live coaching,
- recorded training sessions,
- QA feedback loop.

Repeated employee questions or frustrations are system telemetry and should feed product/process improvement.

## Revenue intelligence

The minimum executive scoreboard is:
1. Lead response time
2. Contact rate
3. Booking rate
4. Show rate
5. Close rate
6. Revenue per lead

Supporting metrics include CPL, CAC, follow-up attempts, missed calls, no-show rate, lost reasons, revenue collected, and leakage by stage.

The system must make the largest revenue leak visible.

## Productization rule

During pilots:

- Needed by **all 3 clients** → core platform candidate.
- Needed by **2 clients** → configurable platform capability candidate.
- Needed by **1 client** → tenant-specific until repeated demand proves otherwise.

This rule protects the platform from premature feature bloat.

## Doctrine test

A Booking Engine implementation is not complete because workflows exist.

It is complete only when a real lead can move through the intended lifecycle, failures are recovered, ownership is clear, the result is measurable, and the final business outcome is achieved.
