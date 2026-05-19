# Tool Adapter Pattern

A tool adapter should be thin.

It can describe:

- where the tool reads instructions;
- how the tool starts a session;
- what local commands it should prefer;
- how it maps tool-specific features to the shared project protocol.

It should not duplicate project policy. Duplicated policy drifts.
