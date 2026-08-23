# Snapshot Instruction: Use Snapshot Dispositions

- **Instruction type:** Snapshot
- **UI verification:** Planned — verify after Snapshot installation

## Outcome

One definitive call result triggers the correct next workflow behavior and produces consistent reporting.

## Canonical disposition set

The deployed set must remain concise enough for the Salesflow account and client workflow design. Map client wording to these outcomes:

- Connected — Booked
- Connected — Expedited, Closed
- Connected — Expedited, Warm Transfer Completed
- Connected — Appointment Protected
- Connected — Progressed, Not Booked
- Connected — Follow-Up Required
- Callback Scheduled
- No Answer or Voicemail
- Disqualified or Not Interested
- Invalid, Wrong Number, or DND

Where the installed Salesflow disposition limit requires consolidation, detailed reasons belong in structured fields or workflow branches—not additional synonymous dispositions.

## Rule

Select the closest definitive outcome. Do not choose a convenient disposition merely to clear the call.
