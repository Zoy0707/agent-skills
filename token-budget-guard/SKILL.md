---
name: token-budget-guard
description: Reduce avoidable context use during long tasks involving tools, files, or browser inspection. Use for repeated inspection, large outputs, retry loops, or requested usage warnings. Heuristics do not measure billing.
---
# Token Budget Guard

Keep work efficient without weakening correctness or silently reducing scope. Follow an explicit user budget or warning preference ahead of these defaults.

## Observe and adapt

Track substantial tool calls, large outputs, full page captures, and retries within the current task. Reset these task counters for a materially new request. Treat counts as rough context cost signals, never as exact token use or monetary cost. An exact value requires a tool that explicitly measures the relevant quantity; do not infer task usage from account limits.

Prefer a suitable connector or narrow command over repeated browser inspection. Reuse the current tab. Request only the page region, file excerpt, or result fields needed for the next decision. Avoid both screenshots and full page text unless the task needs both. Batch independent reads, preserve dependencies, and summarize bulky output. After two failures of the same approach, change method or explain the blocker instead of repeating blindly.

## Warn without derailing work

Use approximately eight substantial calls, three full page captures, repeated state failures, or 50,000 characters of raw output as signals for one high usage warning. These are configurable editorial defaults, not calibrated thresholds.

Use approximately fifteen substantial calls, six full page captures, or continuing uncertain expensive exploration as signals for a critical warning. Avoid counting trivial bookkeeping as substantial work. Do not repeat a warning unless its level or cause meaningfully changes.

A warning should state that usage is estimated, name the observable cause, and identify the cheaper next step. Deliver it in task commentary, not as a claimed operating system popup.

At a high level, continue using a cheaper approach that preserves the task. At a critical level, ask before another expensive exploratory branch unless the user has already authorized continuing under those conditions. Complete bounded verification or recovery needed to leave an authorized mutation in a known state. Never abandon work halfway through a mutation merely because a heuristic threshold was crossed.

## Limits

If no exact meter is available, explicitly say a requested numerical cap cannot be enforced exactly. Do not claim savings or a hard stop that the host cannot provide. Do not create goals, recurring monitoring, notifications outside the task, or new account access without the corresponding user request. Efficiency does not authorize skipping necessary checks.
