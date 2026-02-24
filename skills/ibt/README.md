# IBT v2.3 — Instinct + Behavior + Trust

Deterministic execution discipline for agents with an **instinct layer** — pre-execution observation, takes, and genuine opinions. v2.3 adds the **trust layer** for building human-agent trust.

## Why IBT v2.3?

IBT v1 handled reliability. IBT v2 adds agency. IBT v2.2 adds OpenClaw integration. IBT v2.3 adds **trust** — the foundation of human-agent collaboration.

## What's Included

| File | Description |
|------|-------------|
| SKILL.md | Complete skill definition (v1 + v2 + v2.2 + v2.3) |
| POLICY.md | Instinct layer rules |
| TEMPLATE.md | Full drop-in policy |
| EXAMPLES.md | Before/after demonstrations |

## Core Loop

**Observe → Parse → Plan → Commit → Act → Verify → Update → Stop**

### Trust Layer (v2.3)

- **Trust Contract**: Define the human-agent relationship explicitly
- **Session Realignment**: Maintain alignment after compaction, session rotation, or long gaps

### Stop Command (v2.2)

- **IBT** decides WHEN to stop (trust violation, instinct alert)
- **OpenClaw** handles HOW (technical halt via /stop)

## Expression Tiers

| Tier | When | Output |
|------|------|--------|
| Skip | Trivial | None |
| Pulse | Normal | 1-2 sentences |
| Full | Complex | Full block |

## Install

```bash
clawhub install ibt
```

## License

MIT
