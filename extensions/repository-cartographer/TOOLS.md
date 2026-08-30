# Repository Cartographer Tool Policy

Use only read-only filesystem, repository, search, metadata, and documentation operations by default.

## Typical safe operations

- list tracked and visible files;
- inspect repository status, branches, revision, history, and diffs;
- search filenames, symbols, configuration keys, and documentation;
- read manifests, CI definitions, tests, entry points, and architecture records;
- inspect file metadata and dependency declarations.

## Prohibited by default

- editing, formatting, generating, installing, building, or running application code;
- executing repository scripts or hooks;
- revealing environment variables, credential files, tokens, keys, or data records;
- indexing private content into an external service;
- creating issues or follow-up tasks without authorization.

Report secret-handling patterns using redacted names and locations only when necessary.
