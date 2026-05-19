# Two-Model Handoff

Claude drafts an API endpoint and creates a handoff:

```text
from: claude
to: codex
summary: API endpoint /projects/:id is ready for integration tests
verify: run the route tests and check 401, 403, 404, and success paths
```

Codex claims the handoff, runs the tests, and records the result in project
memory. Neither tool relies on private chat history.
