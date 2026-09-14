# Writing Voice

Helps an agent preserve an author's voice during drafting and revision, using confirmed preferences rather than assumptions.

## Setup

Copy this skill folder into your agent's personal skill directory. Provide a draft and any relevant preferences. A stored profile is optional. If you want persistent learning, explicitly authorize it and choose a private profile location outside this repository.

## Example

```text
Use writing-voice to polish this email. Keep my argument and change only the opening. Do not save any new preferences from this draft.
```

## Input and output

Input is the brief, source text, and optionally a private preference profile or an authorized comparison with the author's revision. Output is the requested text. A concise profile update is possible only when retention is authorized and supported by new evidence.

## Limits

No personal profile is included. The skill does not infer style from typos, treat factual fixes as preferences, or scan accounts for samples. It does not guarantee an author's approval or send content externally.
