# Salesflow Knowledge Center Delivery

## Purpose

Give every employee a searchable, role-based operating manual inside Salesflow without sending them to external documentation.

## Custom menu experience

Add a Salesflow custom menu item named **Booking Engine**.

The landing page should show:

1. **Start My Shift**
2. **My Role**
3. **Appointments**
4. **Live Calls**
5. **Assigned Tasks**
6. **Call Queue**
7. **Recoveries**
8. **Search Actions and Instructions**
9. current Booking Engine and Snapshot versions

Role permissions should hide configuration and maintainer material from ordinary users.

## Page behavior

- Mobile-responsive and usable during calls.
- Search by action, visible Salesflow label, role, phase, path tier, and Recovery.
- Persistent breadcrumb navigation.
- One Action or Salesflow Instruction per page.
- Large numbered steps and short paragraphs.
- Client-specific screenshots placed beside the corresponding step.
- Copy buttons for approved scripts when appropriate.
- Clear escalation action at the bottom of every instruction.
- Version and Last verified metadata visible but unobtrusive.

## Course experience

Use the Salesflow course for structured onboarding, demonstrations, quizzes, certification, and update lessons. Link each lesson to the canonical Role, Action, and Salesflow Instruction used by the Knowledge Center.

## Publishing pipeline

1. Update the repository.
2. Validate links and metadata.
3. Verify clicks inside Salesflow.
4. Add or replace client-specific screenshots.
5. Obtain human review.
6. publish the Knowledge Center and affected course lessons.
7. Display the repository version in Salesflow.

## Drift prevention

- Never maintain an unversioned copy in a separate notebook.
- Never paste an external vendor article as an employee instruction.
- Never duplicate a universal rule inside multiple role pages; link to the canonical rule.
- Record client-specific differences in the client profile and deployment layer.
- Re-verify instructions after interface, permission, workflow, or routing changes.
