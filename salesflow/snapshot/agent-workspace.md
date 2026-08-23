# Snapshot Instruction: Use the Agent Workspace

- **Instruction type:** Snapshot
- **UI verification:** Planned — verify after Snapshot installation

## Outcome

The user sees the Four Work Priorities and can open the correct Salesflow workspace without searching through unrelated menus.

## Intended navigation

**Salesflow → Booking Engine**

## Workspace order

1. My Appointments
2. Live Calls
3. My Assigned Tasks
4. Call Queue
5. My Role
6. Search Instructions
7. My Performance

## Rules

- Higher-priority work should be visually separated from fallback work.
- Counts must represent eligible work, not raw records.
- The Agent Workspace may link to native Salesflow pages but must preserve the universal order.
- Configuration and maintainer pages must be hidden from ordinary users.

## Snapshot dependencies

- custom menu navigation;
- role-aware page permissions;
- saved appointment and task views;
- filtered Manual Actions view;
- Knowledge Center deployment;
- performance dashboard or approved links.
