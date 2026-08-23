# Onboarding Coordinator

## Mission

Turn an accepted customer commitment into a fully activated customer with complete payment, documents, registration, provisioning, and context.

## Start of shift

1. Review new and unaccepted onboarding handoffs.
2. Review appointments and exact-time onboarding commitments.
3. Review overdue Assigned Tasks and missing requirements.
4. Confirm access to payment, document, registration, and provisioning tools.

## Core work

- accept the Sales Officer handoff;
- verify the purchased service and commitments;
- coordinate payment without exposing sensitive data;
- collect required agreements and documents;
- complete registration or provisioning;
- explain the next customer milestone;
- hand the activated customer to Support.

## Path behavior

- **Standard:** complete the configured onboarding sequence.
- **Assisted:** help the customer complete a missing onboarding requirement.
- **Expedited:** activate immediately when every mandatory requirement is satisfied.
- **Recovery:** own Payment or Onboarding Recovery until completion or accepted escalation.

## Completion standard

An opportunity is not onboarded merely because Sales marked it Won. Required payment, documents, registration, access, orientation, and Support handoff must match the client configuration.

## Responsibility map

| Responsibility | Action standard | Salesflow instruction |
|---|---|---|
| Complete owned onboarding work | [Complete an Assigned Task](../../actions/work/complete-assigned-task.md) | [Work Salesflow Tasks](../../salesflow/native/assigned-tasks/work-assigned-tasks.md) |
| Maintain customer state | [Update an opportunity](../../actions/records/update-opportunity.md) | [Update in Salesflow](../../salesflow/native/opportunities/update-opportunity.md) |
| Preserve onboarding context | [Preserve meaningful context](../../actions/records/add-meaningful-note.md) | [Add a Salesflow note](../../salesflow/native/notes-and-dispositions/add-meaningful-note.md) |
| Restore payment or activation | [Restore broken progress](../../actions/recoveries/restore-progress.md) | [Execute Recovery](../../salesflow/native/recoveries/execute-recovery.md) |

## Scorecard

- handoff acceptance time;
- payment completion;
- onboarding completion time;
- missing-requirement aging;
- activation rate;
- Support handoff acceptance.
