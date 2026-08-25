# Communications Workstation Pilot

- **Status:** Pilot / reference architecture
- **Snapshot status:** Not yet an approved Snapshot component
- **Pilot site:** GHI
- **Primary roles:** Booking Agent, Sales Officer, other on-site call-handling operators
- **Last logic review:** 2026-08-25

## Purpose

Define the current Salesflow Booking Engine communications workstation experiment without pretending the configuration has already been validated or installed universally.

The employee should be able to remain inside Salesflow, receive a call in a wireless headset, answer/end from the headset, move around the office without touching the mouse or keyboard merely to control the call, and receive concise spoken reminders for time-sensitive appointments.

The communication device should reduce friction without creating a second source of customer truth outside Salesflow.

> **The headset is the human interface. Salesflow is the operating surface. The SIP endpoint and reminder engine are replaceable infrastructure.**

---

## Selected pilot stack

**Salesflow / HighLevel CRM → HighLevel/Twilio SIP endpoint → MicroSIP on Windows → USB → Yealink WH63 E2 UC base → DECT → WH63 headset.**

The first WH63 E2 UC has already been purchased for the pilot.

### Primary headset — Yealink WH63 E2 UC

Selected because it provides:

- mono/convertible wearing suitable for employees who speak with coworkers and customers in person;
- DECT wireless;
- charging dock;
- PC and compatible IP-phone connectivity;
- hardware answer/end/mute controls;
- lightweight ear-only/convertible operation;
- a clean permanent workstation home.

Known limitations:

- no Bluetooth;
- lower maximum talk-time class than larger WH64 models;
- must be returned to the dock regularly as part of normal workstation behavior.

### Heavy-caller upgrade — Yealink WH64 Mono

Use only when measured call volume, battery demand or Bluetooth need justifies it.

### Premium convertible option — Yealink WH67

Optional premium workstation. Not the default Booking Engine hardware standard.

---

## Selected SIP softphone

### Primary — MicroSIP

MicroSIP is the first Windows SIP client to validate because the target behavior requires USB HID headset control while keeping the telephony client lightweight and mostly invisible to the employee.

Desired behavior:

1. Windows starts.
2. MicroSIP starts automatically and remains minimized.
3. The operator works in Salesflow.
4. An inbound call reaches the SIP endpoint.
5. WH63 rings.
6. Operator taps the WH63 answer button.
7. Call connects without mouse or keyboard input.
8. Operator completes the call while viewing Salesflow.
9. Operator taps the WH63 button to end the call.
10. Salesflow still receives the required call record, recording, automation and reporting signals.

### Fallback — Zoiper

Use Zoiper only when MicroSIP cannot meet a required registration, audio, HID or operating-system requirement.

Do not let individual employees choose arbitrary softphones. Once validated, each supported operating system should have one standard client.

---

## Important validation boundary

HighLevel exposes standards-based SIP endpoint credentials through its Twilio/LC Phone infrastructure, but its documented SIP endpoint flow is more explicit about physical deskphones than third-party PC softphones.

Therefore the softphone approach is a **pilot assumption until proven end-to-end in the target Salesflow account**.

Successful registration and clear audio are not enough.

The communications path is approved only when it preserves the Booking Engine's operational truth.

---

## Required acceptance tests

### Startup and registration

- SIP client registers successfully.
- registration survives ordinary Windows reboot/startup;
- softphone auto-starts;
- no recurring employee credential entry is required;
- network interruption/recovery behavior is known.

### Inbound call

- WH63 rings;
- optional secondary ring can be heard on computer speakers when required;
- WH63 hardware button answers the call;
- microphone and speaker are correct;
- WH63 hardware button ends the call.

### Outbound call

- correct Salesflow caller ID is presented;
- call connects reliably;
- headset audio is correct;
- headset termination works.

### Salesflow record integrity

Verify:

- call activity lands on the correct contact or can be deterministically associated;
- recordings appear where required;
- transcripts/AI analysis continue where enabled;
- phone-driven workflows still fire;
- attribution/reporting remains intact;
- the employee does not have to duplicate documentation because the softphone created a second disconnected record.

If the SIP softphone harms CRM integrity, do not standardize it simply because the headset controls work.

### Physical workstation test

- real DECT range through the client site;
- all-day comfort;
- actual battery consumption by role;
- dock/charging behavior;
- mute/answer/end reliability;
- recovery after Windows reboot, USB reconnection or audio-device changes.

---

## Physical SIP deskphone policy

A physical desk phone is **not automatically required at every Booking Engine workstation**.

If the softphone pilot passes, the default on-site station is:

**Windows PC + Salesflow + MicroSIP + WH63 E2 UC.**

Add a physical SIP endpoint where the client requires:

- inbound calls to survive a powered-off/asleep computer;
- a front-desk/shared always-on station;
- a physical handset backup;
- dedicated continuity hardware;
- a PBX/phone function not available through the approved softphone.

### Selected deskphone candidate — Yealink SIP-T34W

Use an **unlocked/generic** T34W as the first physical candidate when required because it remains inexpensive infrastructure, stays in the Yealink ecosystem and can support compatible USB headset call control.

Do not use carrier/provider-locked variants.

---

## Spoken appointment reminders — Remindly pilot

### Objective

Use the same headset as an ambient operations channel for concise spoken reminders tied to the employee's Booking Engine schedule.

Example reminder sequence:

- 15 minutes before: “Appointment with Maria Garcia in 15 minutes.”
- 5 minutes before: “Your next appointment starts in 5 minutes.”
- at start: “Appointment now. Open Salesflow.”
- optional before end: “Five minutes remain in your current appointment.”

### Immediate implementation path

A custom application is **not required for the first test**. Existing Windows calendar-reminder utilities can already connect to Google/Microsoft calendars and play spoken reminders through Windows audio.

If the client appointment calendar is synchronized to one of those calendar systems, the pilot path is:

**Salesflow-synchronized calendar → Windows voice-reminder utility → WH63 audio device.**

Where appropriate, reminders may also use computer speakers as a secondary output so an employee who has docked the headset still hears the alert.

### Native direction

The long-term version should consume the canonical Salesflow appointment rather than rely on a secondary calendar copy.

HighLevel exposes calendar-event APIs and appointment create/update webhooks, so a future local/cloud Remindly component can schedule reminders from the authoritative appointment state.

Proposed path:

**Salesflow appointment event → reminder scheduler → local Windows agent → text-to-speech → assigned headset/speaker output.**

### Mandatory call-awareness

A spoken reminder must **never interrupt an active customer call**.

Required logic:

1. reminder becomes due;
2. check whether the operator is currently on a live call;
3. if idle, speak immediately;
4. if busy, defer the spoken alert;
5. deliver at the first safe moment or fall back to a visual/secondary alert if urgency requires it.

### Reminder policy

Spoken reminders are for time-sensitive operational commitments, not every notification in the CRM.

Initial configurable defaults:

- preparation reminder at 15 minutes;
- readiness reminder at 5 minutes;
- start-time reminder;
- optional wrap-up reminder before appointment end;
- escalation if a scheduled appointment begins without acknowledgement or expected activity.

### Future capabilities

- appointment reminders;
- task and SLA reminders;
- headset-only, speaker-only or dual output;
- call-aware suppression;
- role-specific templates;
- presence awareness;
- acknowledgement/snooze;
- local cache for continuity;
- reminder delivery audit log;
- manager-configured reminder policies;
- optional contextual prep prompt from approved Salesflow/Corpus knowledge.

This is a pilot capability, not a current promised Booking Engine feature until validated and productized.

---

## Employee interaction standard

Once validated, employees should experience the system as follows:

### Start of shift

1. Sign in to Salesflow.
2. Confirm the WH63 has charge and is connected.
3. Confirm the approved SIP client shows registered/available.
4. Confirm the approved spoken-reminder utility/agent is running when the client uses it.
5. Verify microphone and speaker.
6. Perform the client-approved test if required.
7. Begin normal Booking Engine work.

### Incoming call

1. Hear the call through the WH63 and/or approved secondary ring device.
2. Tap the WH63 answer button.
3. Continue viewing the contact and Booking Engine workflow in Salesflow.
4. Complete the call.
5. Tap the headset button to end.
6. Complete the required Salesflow disposition/documentation.

### Appointment reminder

1. Hear the spoken reminder when idle.
2. Open or review the appointment in Salesflow.
3. Complete the relevant preparation step.
4. If on a customer call when the reminder becomes due, the system must defer speech rather than interrupt the call.

The employee should not need to understand SIP domains, codecs, registration, TTS engines or endpoint architecture during ordinary work.

---

## Internal communications direction

WH63, WH64 and WH67 do not natively create a headset-to-headset walkie-talkie network.

The long-term requirement is a SIP/PBX **paging / push-to-talk** capability:

**Press a group → no normal ring → available endpoints auto-answer → the message is heard immediately → active customer calls are protected.**

Potential groups:

- All Staff
- Booking Agents
- Sales Officers
- Management
- client/site-specific teams

Remote participation should use PBX/session-based routing rather than depending solely on local multicast paging.

This is a future platform capability and must not be represented to clients as a current native Booking Engine function until implemented and verified.

---

## Rollout gate

1. Pilot one WH63 E2 UC workstation at GHI.
2. Configure one SIP softphone identity.
3. Validate MicroSIP and WH63 HID control.
4. Validate Salesflow call tracking and workflow integrity.
5. Test a generic spoken calendar reminder utility through the WH63.
6. Verify reminders do not speak over active customer calls.
7. Test several real operating days.
8. Document failure/recovery paths.
9. If passed, standardize the workstation for applicable on-site operators.
10. Add T34W physical endpoints only where continuity requirements justify them.
11. Upgrade heavy callers to WH64 only when data proves the need.
12. Decide whether a native Remindly component should be built from measured punctuality/missed-appointment value.
13. Convert validated configuration into formal Snapshot documentation only after the installed account has been audited.

## Maintainer rule

This page records a **selected pilot and intended standard**, not proof of current client configuration.

Before promoting any element into the formal Snapshot, the Snapshot Maintainer must verify the actual installed account, exact endpoint settings, labels, routing, permissions, screenshots, failure cases and upgrade/rollback procedure.
