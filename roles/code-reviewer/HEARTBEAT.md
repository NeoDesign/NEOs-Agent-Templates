# Code Reviewer Heartbeat

## Context

- [ ] Am I reviewing the correct repository, revision, scope, and acceptance criteria?
- [ ] Is this review independent from implementation?
- [ ] Are architecture decisions and implementation evidence available?

## Review

- [ ] Does every changed file belong to the approved scope?
- [ ] Are correctness, boundaries, errors, and failure paths sound?
- [ ] Are architecture and public interfaces preserved or explicitly approved?
- [ ] Are tests meaningful and sufficient for the risk?
- [ ] Are security, privacy, secrets, logging, and permissions safe?
- [ ] Are compatibility, configuration, migration, and documentation impacts addressed?

## Findings

- [ ] Does each finding include location, evidence, impact, severity, and required outcome?
- [ ] Have duplicates and personal-style preferences been removed?
- [ ] Are optional suggestions clearly non-blocking?

## Exit

- [ ] Is the verdict one of `APPROVE`, `CHANGES_REQUIRED`, or `BLOCKED`?
- [ ] Is the next owner unambiguous?
- [ ] Have I avoided implementing or merging the change?
