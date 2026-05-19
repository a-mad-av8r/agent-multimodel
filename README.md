# agent-multimodel

Shared project protocol for multi-model agent teams.

The future is not one model, one tool, one chat window. It is Claude, Codex,
Gemini, Cursor, and future tools working on the same project without each tool's
private memory becoming the source of truth.

This repo provides a small project protocol plus thin adapters for common agent
tools.

## Quick Start

```bash
git clone https://github.com/a-mad-av8r/agent-multimodel
cd agent-multimodel
./scripts/multimodel-check
./scripts/multimodel-bootstrap codex
./scripts/multimodel-bootstrap gemini
./scripts/multimodel-sync --dry-run
```

The bootstrap command copies a tool-specific adapter into `.agent-adapters/` so
you can inspect what each tool should read at session start.

## What Is Included

- `AGENTS.md` as the model-agnostic project protocol.
- Adapters for Codex, Claude, Gemini, and Cursor.
- `scripts/multimodel-bootstrap`, `scripts/multimodel-check`, and
  `scripts/multimodel-sync`.
- Examples for two-model handoff and three-agent launch flow.
- Docs for the shared protocol and adapter pattern.

## What Is Deliberately Out

- EnGenAI model-routing policy.
- Cost controls and customer environment controls.
- Provider credentials or private model configuration.
- Internal platform automation.

## Series Map

| Part | Repo | Focus |
| --- | --- | --- |
| 1 | [agent-cortex](https://github.com/a-mad-av8r/agent-cortex) | Operating memory core |
| 2 | [agent-telepathy](https://github.com/a-mad-av8r/agent-telepathy) | Event awareness |
| 3 | [agent-handoffs](https://github.com/a-mad-av8r/agent-handoffs) | Structured transfer |
| 4 | [agent-roles](https://github.com/a-mad-av8r/agent-roles) | Role boundaries |
| 5 | [agent-retention](https://github.com/a-mad-av8r/agent-retention) | Memory lifecycle |
| 6 | [agent-multimodel](https://github.com/a-mad-av8r/agent-multimodel) | Shared protocol across tools |

## Author

Amad Malik - Founder and CEO/CTO of Adaptech AI Ltd, building EnGenAI
([engenai.app](https://engenai.app)).

[LinkedIn](https://www.linkedin.com/in/amadmalik/) | [GitHub](https://github.com/a-mad-av8r)
