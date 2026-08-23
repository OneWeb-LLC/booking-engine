# Native Field Map

This map will record standard Salesflow fields used by the Snapshot.

| Concept | Native object or field | Source of truth | Notes |
|---|---|---|---|
| Contact identity | Contact | Salesflow Contact | Do not duplicate identity in custom fields |
| Assigned owner | Contact or Opportunity owner | Salesflow assignment | Ownership must be accepted |
| Appointment status | Appointment status | Salesflow Calendar | Attendance is separate from sales outcome |
| Opportunity stage | Pipeline stage | Salesflow Opportunity | Current lifecycle state |
| Opportunity status | Open, Won, Lost, or approved terminal state | Salesflow Opportunity | Terminal commercial status |
| Call outcome | Call disposition | Salesflow call record | One definitive outcome |
| Personal responsibility | Task owner and due time | Salesflow Task | Exact-time callbacks are appointments |

The Salesflow Administrator must verify the final visible labels and object behavior before the Snapshot is published.
