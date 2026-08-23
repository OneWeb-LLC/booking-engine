# UI Verification Standard

Click-by-click Salesflow instructions are trustworthy only when the visible Salesflow interface matches the page.

## Verification states

- **Draft:** logic written but not tested in Salesflow.
- **Verified:** completed successfully in the designated test account.
- **Client Verified:** confirmed with that client's permissions, labels, and configuration.
- **Review Required:** interface or workflow change may have invalidated the instruction.

## Verification checklist

1. Use a non-production test contact when practical.
2. Sign in with the same permission level as the target role.
3. Follow every step exactly as written.
4. Confirm visible labels, navigation, buttons, fields, and statuses.
5. Confirm downstream messages, workflows, routing, and suppression.
6. Test at least one failure or Recovery path.
7. Capture Salesflow-branded screenshots without unnecessary personal or sensitive data.
8. Record account, role, verifier, date, and result.
9. Mark affected instructions Client Verified only after client-specific labels and permissions are confirmed.

## Screenshot standard

- Capture only the area needed for the step.
- Use a test contact and redact unnecessary identifiers.
- Show the visible label being clicked.
- Add a numbered callout when the target is not obvious.
- Store screenshots beside the instruction or in its client deployment asset folder.
- Replace screenshots rather than accumulating obsolete versions in the employee experience.

## Review triggers

- navigation redesign;
- renamed button or page;
- new role or permission behavior;
- workflow or disposition change;
- calendar, pipeline, or routing change;
- employee reports that the instruction no longer matches Salesflow.
