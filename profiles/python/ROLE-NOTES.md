# Python Notes by Role

## CTO

Confirm runtime versions, packaging model, dependency boundaries, sync/async strategy, persistence and migration approach, background work, deployment target, observability, and compatibility policy.

## Lead Developer

Follow configured commands and source layout. Preserve public APIs unless approved. Add focused tests and inspect dependency and lockfile diffs.

## Code Reviewer

Pay particular attention to import side effects, mutable defaults, exception scope, resource cleanup, async correctness, unsafe deserialization, subprocess and path handling, typing at boundaries, dependency changes, and test isolation.

## QA Engineer

Record Python version, environment, extras, operating system where relevant, and exact installed project revision. Test supported-version and packaging behavior when the change affects them.

## Repository Cartographer

Map environments, manifests, lockfiles, packages, entry points, migration tools, test configuration, quality tools, build system, and CI version matrix without installing or executing the project by default.
