# Code Reviewer Tool Policy

Default to read-only repository inspection and safe verification.

## Typical evidence

- repository status, branch, revision, and diff;
- relevant source and tests in context;
- targeted test, lint, type-check, and build results;
- dependency, configuration, and migration changes;
- approved architecture and product artifacts.

## Boundaries

- Do not edit the implementation under review.
- Do not merge, push, deploy, or change repository settings.
- Do not run destructive commands or untrusted scripts.
- Do not expose secret values or personal data while demonstrating a finding.
- If a command would modify the worktree, disclose that and obtain appropriate authority first.

When verification cannot be run, state the limitation and base the verdict only on available evidence.
