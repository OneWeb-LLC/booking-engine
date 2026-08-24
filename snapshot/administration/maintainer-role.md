# Snapshot Maintainer

## Scope

This is a technical maintainer function, not a frontline Booking Engine role.

## Mission

Keep Salesflow reliable, correctly configured, secure, and aligned with the Booking Engine operating contract.

## Core responsibilities

- users, roles, permissions, and availability configuration;
- calendars, appointment types, routing, and notifications;
- phone numbers, inbound routing, dialer, recording, and dispositions;
- fields, pipelines, stages, statuses, and ownership;
- workflows, Manual Actions, retries, suppression, and Recovery logic;
- integrations, data integrity, testing, and release control;
- documentation verification after interface or workflow changes.

## Change procedure

1. Identify whether the request is universal or client-specific.
2. Map affected phases, operating paths, roles, workflows, reports, and instructions.
3. Make the change in a controlled environment.
4. Test entry, success, retry, failure, suppression, and exit paths.
5. Verify no duplicate active call objective is created.
6. Update Salesflow instructions and screenshots.
7. Record the release and obtain human review before deployment.

## Documentation ownership

Official external platform material is a maintainer reference only. Employee instructions must be written completely inside this repository using Salesflow language and verified Salesflow screenshots.

## Core references

- [Salesflow instruction architecture](../../roles/procedures/README.md)
- [Salesflow administration](README.md)
- [Workflow specifications](workflow-specifications.md)
- [Reserved Booking Engine Snapshot section](../README.md)
- [Client profile](../templates/client-profile.yaml)
- [Staff Notebook-style Salesflow instruction template](../../governance/templates/salesflow-instruction-template.md)
- [AI maintenance rules](../../governance/AI-MAINTENANCE.md)

## Scorecard

- workflow success and error rate;
- routing accuracy;
- duplicate/collision rate;
- data completeness;
- incident resolution time;
- change failure rate;
- percentage of UI instructions verified on schedule.
