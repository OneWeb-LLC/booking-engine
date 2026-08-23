# Living Wiki Architecture

## Canonical page types

| Page type | Question answered | May contain exact clicks? |
|---|---|---|
| Methodology | Why does the system work this way? | No |
| Role | Who owns this and what authority do they have? | Link only |
| Salesflow Instruction | What outcome is required and exactly how is it completed? | Yes |
| Snapshot | What configuration implements the behavior? | Administrator detail |
| Training | How is competency developed and tested? | Links to canonical pages |
| Governance | How is the wiki maintained and trusted? | Maintainer detail |

## Link direction

The preferred path is:

**Role → Salesflow Instruction → Configuration Dependency**

Reverse links may provide context, but no lower layer may redefine a higher-layer rule.

## Canonical-source rule

- A universal rule is written once in Methodology.
- A responsibility is written once in the owning Role.
- An outcome standard and visible click path are written once as a Salesflow Instruction.
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

- **Employee:** Roles, approved Salesflow Instructions, Recoveries, and Training.
- **Manager:** Employee content plus Methodology and management pages.
- **Administrator:** All operational content plus Snapshot and Administration.
- **Maintainer:** Entire repository, Governance, and vendor References.
