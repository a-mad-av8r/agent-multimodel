# Shared Project Protocol

The project is the source of truth.

Each tool can have a local adapter, but the adapter must point back to shared
project state:

- memory for durable decisions and lessons;
- handoffs for ownership transfer;
- roles for boundaries;
- local checks for verification.

The failure mode this prevents is split-brain operation: each model thinks it
knows the project because each model has its own private context.
