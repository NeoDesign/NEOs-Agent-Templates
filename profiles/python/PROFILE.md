# Python Development Profile

Apply this profile in addition to a role definition. Repository-local instructions take precedence for concrete commands and versions. This profile does not enlarge the role's authority.

## Discover before assuming

Inspect the repository for:

- `pyproject.toml`, `requirements*.txt`, `setup.cfg`, `setup.py`, `Pipfile`, `poetry.lock`, `uv.lock`, or other environment definitions;
- supported Python versions and operating systems;
- source layout such as `src/`, packages, services, notebooks, and scripts;
- test, lint, formatting, type-check, build, and documentation configuration;
- CI commands that represent the project's required checks.

Do not introduce a new package manager or toolchain merely because it is preferred here.

## Implementation principles

- Follow the project's supported Python version and established style.
- Use clear types at public boundaries; do not add noisy annotations without value.
- Prefer explicit data flow and dependency injection over hidden global state.
- Keep modules cohesive and imports free of unintended side effects.
- Preserve synchronous or asynchronous conventions already chosen by the architecture.
- Validate untrusted input at system boundaries.
- Handle resources with context managers and define timeouts for external operations.
- Avoid broad exception handling; preserve causal context and actionable error messages.
- Do not log secrets, credentials, tokens, or unnecessary personal data.
- Keep configuration external to code and fail safely when required configuration is absent.

## Dependencies

Add a dependency only when it provides clear value over the standard library or existing dependencies. Check compatibility, maintenance status, license expectations, security posture, transitive cost, and lockfile impact. Dependency installation and network access require appropriate authorization.

## Testing

Use the repository's test framework, commonly `pytest` or `unittest`. Test observable behavior, boundary conditions, errors, permissions, and regression scenarios. Keep tests deterministic and isolated from real external services. Use fixtures deliberately; avoid coupling tests to private implementation details without reason.

## Quality commands

Use only tools configured by the repository. Common examples, not defaults:

```text
pytest
ruff check .
ruff format --check .
mypy .
pyright
python -m build
```

Run targeted checks first. Do not run a broad formatter across unrelated files.

## Security and privacy

- Use parameterized database access and safe serializers.
- Treat subprocesses, archives, paths, templates, and deserialization as trust boundaries.
- Pin or lock dependencies according to project policy.
- Never commit `.env` files, credentials, keys, production data, or raw sensitive logs.
- Prefer synthetic fixtures and redacted error evidence.

## Python definition of done

- The change supports the declared Python versions.
- Relevant tests pass and failure paths are covered proportionately.
- Configured formatting, linting, typing, and build checks pass or limitations are reported.
- Dependency and lockfile changes are intentional.
- Public behavior and configuration changes are documented.
- No debug artifacts, generated clutter, secrets, or unrelated formatting remain.
