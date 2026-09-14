# Token Budget Guard

Helps an agent notice repeated inspection and oversized output, then choose a narrower way to continue.

## Setup

Copy this skill folder into your agent's personal skill directory. No external account is required. The agent must have access to its current task context. Exact token measurement requires a separate meter provided by the host.

## Example

```text
Use token-budget-guard while investigating this issue. Warn me when repeated inspection becomes expensive, and use narrow reads where possible.
```

## Input and output

Input is the current task and any user budget or warning preference. Output is a compact warning when warranted, together with a cheaper next step. It does not produce a billing report.

## Limits

Default thresholds are heuristics. This skill cannot guarantee a spending cap, create a native popup, or prove token savings. Necessary correctness checks still apply.
