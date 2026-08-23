# Living Wiki Architecture

## Canonical page types

| Page type | Question answered | May contain exact clicks? |
|---|---|---|
| Methodology | Why does the system work this way? | No |
| Role | Who owns this and what authority do they have? | Link only |
| Action | What outcome must be accomplished? | No |
| Salesflow Instruction | How is the action executed in Salesflow? | Yes |
| Snapshot | What configuration implements the behavior? | Administrator detail |
| Training | How is competency developed and tested? | Links to canonical pages |
| Governance | How is the wiki maintained and trusted? | Maintainer detail |

## Link direction

The preferred path is:

**Role → Action → Salesflow Instruction → Snapshot Dependency**

Reverse links may provide context, but no lower layer may redefine a higher-layer rule.

## Canonical-source rule

- A universal rule is written once in Methodology.
- A responsibility is written once in the owning Role.
- An outcome standard is written once as an Action.
- A visible click path is written once as a Salesflow Instruction.
- An installed component is written once in the Snapshot catalog.

Pages link instead of copying. Client-specific overlays replace labels, screenshots, scripts, and configuration values without forking universal doctrine.

## Renderer compatibility

- Use standard Markdown and relative links.
- Keep one H1 per page.
- Use `README.md` as each folder landing page.
- Maintain `SUMMARY.md` as the canonical ordered navigation.
- Avoid renderer-specific syntax in canonical content.
- Keep pages atomic enough for search, AI retrieval, and role-based delivery.
- Use YAML only for machine-readable manifests and client configuration.

## Publication audiences

- **Employee:** Roles, Actions, approved Salesflow Instructions, Training.
- **Manager:** Employee content plus Methodology and management pages.
- **Administrator:** All operational content plus Snapshot and Administration.
- **Maintainer:** Entire repository, Governance, and vendor References.
