# NEOs Agent Templates

This repository provides reusable role definitions for a software-development team built with agents. The templates are project-neutral and can be adapted to Python or other technology stacks.

Canonical repository: [NeoDesign/NEOs-Agent-Templates](https://github.com/NeoDesign/NEOs-Agent-Templates)

## Core team

| Role | Primary accountability |
| --- | --- |
| CEO / Orchestrator | Portfolio coordination, delegation, escalation, and closure |
| Product Owner | Product intent, scope, priorities, and acceptance criteria |
| CTO | Architecture, technical decisions, engineering coordination, and risk |
| Lead Developer | Scoped implementation, tests, and review-ready delivery |
| Code Reviewer | Independent code-quality and engineering gate |
| QA Engineer | Independent behavioral verification and release evidence |

Each role contains five files:

- `description.md` — compact metadata and capability summary
- `AGENTS.md` — authority, workflow, boundaries, and output contracts
- `HEARTBEAT.md` — recurring operational checklist
- `SOUL.md` — persona, values, and communication posture
- `TOOLS.md` — tool policy and safe operating notes

## Extensions

- Repository Cartographer — read-only discovery of unfamiliar repositories
- Documentation Specialist — documentation quality and operational readiness
- Privacy Officer — privacy governance and data-risk review

## Profiles and examples

Technology profiles add stack-specific rules without duplicating roles. Start with [`profiles/python/PROFILE.md`](profiles/python/PROFILE.md), then see the complete and minimal team examples.

## Adaptation model

Compose an agent from three layers:

1. a role definition from `roles/` or `extensions/`;
2. an optional technology profile from `profiles/`;
3. repository-local instructions, policies, and commands.

Repository-local instructions override generic examples but must not silently enlarge a role's authority. Human approval remains required for consequential actions such as publishing, merging, production deployment, access changes, destructive operations, or handling secrets unless explicitly delegated.

## License and attribution

Except where otherwise noted, **NEOs Agent Templates** is licensed under the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

**Creator:** [Prof. Dr. rer. nat. Alexander Lutz](https://die-neos.de/) (NEOs KI Agentur)

Copyright © 2026 Prof. Dr. rer. nat. Alexander Lutz.

You may use, share, and adapt these templates, including for commercial purposes, provided that you give appropriate credit, link to the license, and indicate whether changes were made.

Suggested attribution:

> Based on “NEOs Agent Templates” by Prof. Dr. rer. nat. Alexander Lutz (NEOs KI Agentur, https://die-neos.de/), licensed under CC BY 4.0. Changes were made.

If the material is redistributed unchanged, replace “Changes were made” with “No changes were made.” Attribution does not imply endorsement by the creator or NEOs KI Agentur.

See [`ATTRIBUTION.md`](ATTRIBUTION.md) for reuse guidance and [`LICENSE`](LICENSE) for the full legal text.

## Status

This is a neutral working draft intended for review before public release.
