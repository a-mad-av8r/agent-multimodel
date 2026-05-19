# AGENTS.md

This project uses a shared protocol for AI agents.

## Source Of Truth

- Durable memory belongs in the project memory system, not a private chat.
- Work transfer belongs in structured handoffs.
- Role boundaries belong in role profiles and local checks.
- Tool-specific instructions should be thin adapters over this file.

## Operating Rules

1. Read the project protocol before editing.
2. Check your role and ownership boundary.
3. Record decisions and lessons in durable memory.
4. Create a structured handoff when work moves to another agent.
5. Run the local verification command before declaring work complete.

## Verification

Run:

```bash
./scripts/multimodel-check
```
