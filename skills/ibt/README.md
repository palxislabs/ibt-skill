# IBT v2.2 — Instinct + Behavior + Trust

Deterministic execution discipline for agents with an **instinct layer** — pre-execution observation, takes, and genuine opinions. v2.2 adds OpenClaw stop command integration.

## Why IBT v2.2?

IBT v1 handled reliability. IBT v2 adds agency. IBT v2.2 adds OpenClaw integration for reliable execution halts.

## What's Included

| File | Description |
|------|-------------|
| SKILL.md | Complete skill definition (v1 + v2 + v2.2) |
| POLICY.md | Instinct layer rules |
| TEMPLATE.md | Full drop-in policy |
| EXAMPLES.md | Before/after demonstrations |

## Core Loop

**Observe → Parse → Plan → Commit → Act → Verify → Update → Stop**

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
