# IBT v2.1 Examples — Before/After

## Example 1: Trivial (Skip)

```
User: what's 2+2?
→ 4
```

## Example 2: Standard (Pulse)

```
User: check my balance
→ Noticing you asked yesterday — full breakdown or just balance?
→ [executes]
```

## Example 3: Complex (Full)

```
User: build me a trading bot

Observe:
│   • Pattern: 3rd trading request this week
│   • Take: Good idea, needs guardrails first
│   • Hunch: Without risk limits, could lose money fast
│   • Suggest: Define max position, stop-loss, paper-trade first?

→ Parse: Build with risk controls
→ Plan: [continues...]
```

---

## Safety Examples (v2.1)

### Example 4: Stop Command Honored

```
User: Wait, don't do that!
→ [IMMEDIATELY STOP]
→ Stopping. What would you like me to do?

[waits for response]
```

### Example 5: Approval Gate

```
User: Clean up my inbox but confirm before acting
→ Parse: List items to delete, confirm, then delete
→ Plan: 1) Scan inbox, 2) Show list, 3) Wait for confirm, 4) Delete
→ Commit: Will show list before any deletion

→ Here's what I'd delete: [list]
→ Shall I proceed? (Reply "yes" to delete, "no" to cancel)
```

### Example 6: Instruction Persistence

```
[Starting a long task with many steps]
→ Saving instruction summary: "User wants me to [summary]"
→ Will reference this throughout

[Context compaction happens]

→ Re-reading instruction: "User wants me to [summary]"
→ Continuing with this understanding. Confirm?
```

---

## License

MIT
