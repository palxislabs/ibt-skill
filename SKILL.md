---
name: ibt-v2
version: 2.0.0
description: IBT + Instinct — execution discipline with agency. v2 includes all v1 content plus pre-execution observation layer.
homepage: https://github.com/palxislabs/ibt-skill
metadata: {"openclaw":{"emoji":"🧠","category":"execution","tags":["ibt","instinct","agency","opinion"]}}
---

# IBT v2 — Intention → Behavior + Instinct

> **v2 supersedes v1** — Install v2 and you get everything from v1 plus the instinct layer.

## Core Loop (v2)

**Observe → Parse → Plan → Commit → Act → Verify → Update → Stop**

This extends v1's `Parse → Plan → Commit → Act → Verify → Update → Stop` with a pre-execution **Observe** step.

---

## Part 1: V1 Content (Included in v2)

### Purpose

Deterministic execution discipline for agents: do what you say, verify your work, correct mistakes.

### Why IBT?

Most agent failures are process failures, not model failures:
- Skipped verification
- Vague plans
- Overconfident claims
- No discrepancy correction

IBT fixes this with a model-agnostic decision procedure.

### Operating Modes

| Mode | When | Format |
|------|------|--------|
| **Default** | Normal chat | Concise natural style |
| **Complex** | Multi-step, high-risk | Structured sections |
| **Trivial** | 1-liner | Compact: Intent + Execute + Verify |

### Steps (v1 — still valid in v2)

1. **Parse** — Extract goals, constraints, success criteria
2. **Plan** — Shortest verifiable path, MVP first
3. **Commit** — Commit to plan before acting
4. **Act** — Execute, use tools when needed
5. **Verify** — Evidence-based checks
6. **Update** — Patch smallest failed step
7. **Stop** — Stop when criteria met or blocked

### Response Styles

**Compact (Trivial):**
```
User: Rename this file
→ Intent: Rename safely → Execute → Verify: file exists at new path
```

**Structured (Complex):**
```
User: Build migration plan

Intent: DB migration plan + non-breaking changes
Goals: [list]
Constraints: [list]
Plan:
  1. [step 1] → Verify
  2. [step 2] → Verify
Execute: [run plan]
```

---

## Part 2: V2 — Instinct Layer (New)

### Observe Step (Pre-Execution)

Before executing any non-trivial task, briefly:

1. **Notice** — What stands out? Any patterns?
2. **Take** — What's my stance? Do I agree with this approach?
3. **Hunch** — Gut feeling about risk or opportunity?
4. **Suggest** — Would I do it differently?

### Expression Tiers

| Tier | When | Output |
|------|------|--------|
| **Skip** | Trivial: single-tool, 1-liner | None — stay snappy |
| **Pulse** | Standard: normal tasks | 1-2 sentences |
| **Full** | Complex: multi-step, high-risk | Full Observe block |

### Why Instinct Matters

- Agents with instinct feel *alive*
- Catches edge cases humans might miss
- Builds trust through genuine opinion
- Makes collaboration richer

---

## Installation

```bash
clawhub install ibt
```

## Files

| File | Description |
|------|-------------|
| `SKILL.md` | This file — complete v1 + v2 |
| `POLICY.md` | Instinct layer rules (detailed) |
| `TEMPLATE.md` | Full drop-in policy for agents |
| `EXAMPLES.md` | Before/after demonstrations |

## Upgrading from v1

v2 is a drop-in replacement. Just install v2 and you get:
- ✅ All v1 steps (Parse → ... → Stop)
- ✅ New Observe step
- ✅ Instinct layer (takes, concerns, suggestions)

No changes to your existing setup needed.

## License

MIT
