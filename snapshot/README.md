# Booking Engine Snapshot

This section is intentionally reserved for the installable Salesflow configuration that will implement the Booking Engine methodology.

## Status

**Reserved — no Snapshot has been documented or approved.**

Do not treat planned fields, workflows, pipelines, calendars, dispositions, routing, navigation, dashboards, identifiers, communications endpoints, or reminder utilities as installed components. When the final Snapshot is created, an implementation agent must audit the actual account and build this section from observed configuration.

## Active pilots / reference architecture

- [Communications Workstation Pilot](communications-pilot.md) — selected GHI experiment for WH63 E2 UC + MicroSIP + HighLevel/Twilio SIP, conditional physical deskphones, internal paging direction, and spoken appointment reminders (“Remindly”).

Pilot documentation records a selected experiment and acceptance criteria. It does **not** mean the capability is an approved Snapshot feature or a client promise.

The future audit must document:

- the exact exported components and identifiers;
- core capabilities used instead of custom replacements;
- installation order and prerequisites;
- verification tests for entry, success, retry, failure, suppression, and exit;
- upgrade and rollback procedures;
- the corresponding employee instructions and screenshots;
- the independently versioned Snapshot release.

## Design rules

- Prefer core Salesflow objects before creating custom replacements.
- Custom fields must represent durable state or required workflow input.
- Every workflow must map to a methodology transition and named owner.
- Every component must have an installation, verification, upgrade, and rollback note.
- Client-specific values belong in configuration, not universal workflow logic.
- Experimental hardware/software must remain explicitly marked as pilot until validated in the target account.
