# Snapshot Workflow Catalog

Workflow specifications define behavior. Exported or installed workflows will be recorded here after the Snapshot is created.

## Planned workflow families

| ID | Workflow | Primary transition |
|---|---|---|
| WF-01 | New Lead Activation | Capture → Convert |
| WF-02 | Missed Inbound Call | Live demand → Recovery |
| WF-03 | Appointment Protection | Convert milestone protection |
| WF-04 | Assigned Callback | Exact-time commitment |
| WF-05 | Call Queue Retry | Failed pooled call → next attempt |
| WF-06 | Reactivation | Dormant eligible opportunity → Convert |
| WF-07 | Path Orchestration | State recheck and strongest valid objective |
| WF-08 | Conversion Recovery | Unresolved Close decision |
| WF-09 | Payment Recovery | Commitment → completed commercial action |
| WF-10 | Onboarding Recovery | Close → activated customer |

See the [behavior specifications](../../salesflow/administration/workflow-specifications.md).

## Workflow entry contract

Every installed workflow must record:

- installed name and identifier;
- version;
- trigger and filters;
- writers and fields changed;
- user-facing work created;
- collision and suppression checks;
- success, retry, failure, exit, and escalation paths;
- dependent instructions and reports;
- test evidence and rollback behavior.
