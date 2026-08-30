# Composition Example

For each agent, load instructions in this order:

## CEO

1. `roles/ceo/AGENTS.md`
2. `roles/ceo/SOUL.md`
3. `roles/ceo/TOOLS.md`
4. repository-local governance

## Product Owner

1. `roles/product-owner/AGENTS.md`
2. `roles/product-owner/SOUL.md`
3. `roles/product-owner/TOOLS.md`
4. repository-local product context

## Engineering roles

For CTO, Lead Developer, Code Reviewer, and QA Engineer:

1. the role's `AGENTS.md`;
2. the role's `SOUL.md`;
3. the role's `TOOLS.md`;
4. `profiles/python/PROFILE.md`;
5. `profiles/python/ROLE-NOTES.md`;
6. repository-local instructions and commands.

Use each role's `HEARTBEAT.md` as a recurring checklist, not as a replacement for the main role contract.
