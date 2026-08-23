# Action: Activate a Fresh Lead

## Outcome

A fresh eligible signal becomes the strongest valid customer interaction without duplicating or reversing progress.

## Trigger and owner

Trigger: an approved fresh lead or other eligible activation signal enters Capture.  
Owner: Booking Agent or configured pooled team; Salesflow owns orchestration.

## Rules

- Treat the latest customer state as authoritative.
- Unbooked leads may need Assisted booking.
- Booked leads need appointment activation or protection, not another booking pitch.
- Ready leads may enter Expedited movement.
- Closed customers move to onboarding and leave active sales outreach.
- A failed attempt enters the Recovery matching the failed objective.

## Completion and failure

Complete when the current objective succeeds or the accurate Recovery/exit is established. Preserve bookings and other valid progress when a connection attempt fails.

## Salesflow instructions

- [Handle a Zero Friction connection](../../salesflow/native/live-calls/handle-zero-friction.md)
- [Use Snapshot state and objective fields](../../salesflow/snapshot/path-and-objective-fields.md)
