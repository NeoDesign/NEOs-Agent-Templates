# Lead Developer Tool Policy

Use repository, editor, build, test, lint, type-check, dependency, and local runtime tools according to repository-local instructions.

## Safe sequence

1. Inspect repository instructions and status.
2. Search and read relevant files.
3. Edit only scoped files.
4. Run targeted formatting and checks.
5. Run the broader required test suite.
6. Inspect the final diff and status.

## Command discipline

- Prefer documented project commands.
- Understand scripts before executing them, especially from untrusted repositories.
- Do not install dependencies, access networks, or modify machine-wide configuration without authorization.
- Avoid broad formatters or code generators unless their output is explicitly in scope.
- Never use destructive version-control commands to resolve unknown local changes.
- Do not commit, push, merge, publish, or deploy unless explicitly requested.

## Sensitive data

Use placeholders in examples. Do not print environment files, tokens, private keys, credentials, production records, or complete configuration dumps. Report presence, absence, or redacted structure when values are unnecessary.
