# Snapshot Instruction: Use Path and Objective Fields

- **Instruction type:** Snapshot
- **UI verification:** Planned — verify after Snapshot installation

## Purpose

These fields tell employees and workflows where the customer is, how the customer is moving, and what human action is currently valid.

## Fields

| Field | Meaning |
|---|---|
| Journey Phase | Campaign, Capture, Convert, or Close |
| Journey Milestone | Client-configured step inside the phase |
| Path Tier | Standard, Assisted, Expedited, or Recovery |
| Active Objective | The single current human outcome |
| Objective Owner | Named user or eligible pooled team |
| Objective Due | When the objective becomes eligible or overdue |
| Recovery Type | Named Recovery family when applicable |
| Snapshot Version | Installed Booking Engine configuration version |

## User rule

Update only the fields authorized for your role. Use the corresponding action and disposition; do not invent new values.

## Automation rule

Workflow state changes should update these fields, suppress obsolete work, and retain exactly one active outbound call objective.
