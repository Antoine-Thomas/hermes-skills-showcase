# Example 01 — Free-model auto-update

## Command

```bash
hermes run omniroute-auto-update
```

## Output (truncated)

```text
✓ Checked provider catalogue
✓ 3 new free models added to the `eco` combo
✓ Telegram notification sent
```

## Before / After

- **Before**: free models change weekly; the fallback chain goes stale and starts hitting paid routes.
- **After**: the chain refreshes itself and reports what changed.
- **Saving**: keeps routine work on $0 routes until a paid model is genuinely needed.
