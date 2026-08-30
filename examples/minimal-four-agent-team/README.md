# Minimal Four-Agent Team

This reduced team is suitable for small educational projects and prototypes.

## Roles

1. CEO / Orchestrator
2. Product Owner
3. CTO / Lead Developer
4. Code Reviewer / QA Engineer

## Composition rules

When combining CTO and Lead Developer, the agent may design and implement, but consequential architecture decisions must still be explicit and reviewable.

When combining Code Reviewer and QA, preserve two separate passes:

1. code and engineering review;
2. behavioral acceptance verification.

The combined reviewer must remain independent from the combined CTO/Developer. It must issue separate engineering and QA verdicts and must not implement fixes.

## When not to use this model

Use the complete six-role team when the system is safety- or privacy-sensitive, has several developers, changes public interfaces, includes migrations or production operations, or benefits from clearly independent quality gates.
