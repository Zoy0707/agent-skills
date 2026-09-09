---
name: master-prompt-builder
description: Turn rough software ideas into clarified requirements and a durable coding-agent project constitution. Use for PRDs, project kickoff prompts, or master prompts; not one-off feature implementation.
---
# Master Prompt Builder

Produce two artifacts: implementation-ready requirements, then a project constitution that a new coding agent can use without chat history. Do not start implementation unless requested.

## Clarify requirements

Extract confirmed goals, actors, core journeys, business rules, ownership, permissions, data lifecycle, integrations, constraints, and exclusions. Keep guesses separate from confirmed facts.

Ask a small batch of consequential questions: questions whose answers could change the core workflow, data ownership, permissions, retention, billing, or major architecture. Defer cosmetic choices. If an answer already exists in the provided material, reuse it.

Do not mark requirements ready while unresolved product choices could invalidate the foundation. Implementation details can remain TBD when they do not alter product behavior. If the user requests a provisional draft, label it PROVISIONAL and identify exactly which dependent work must wait.

Write requirements using `references/requirements.md`, omitting irrelevant sections. Preserve the user's stated constraints and distinguish Confirmed, Deferred/TBD, Future Scope, and Out of Scope.

## Create the project constitution

When consequential product decisions are resolved, produce a self-contained English document with:

- Product purpose, intended users, and the smallest complete MVP flow.
- Roles, ownership, functional domains, business rules, and data lifecycle.
- Scope and exclusions.
- Decisions classified as Locked (explicitly confirmed), Preferred (open to justified revision), or TBD (unresolved). Do not promote preferences into commitments.
- Known integration, security, and operational constraints. Do not invent vendors, authentication methods, or retention policies.
- Agent working rules: inspect existing repository state; preserve unrelated work; update relevant product, decision, and progress documents after meaningful changes.
- A minimal documentation map. Add feature documents or implementation plans only when they serve current work; do not prescribe an empty documentation hierarchy.
- Development phases appropriate to the project, the current phase, and conditions for advancing.
- One bounded current task and observable completion criteria.

Respect authorization already provided by the user. Do not invent repeated approval gates for routine work. For unresolved consequential decisions, explain the alternatives and ask only what is needed. Verify changing technical facts against current official documentation when selecting technologies.

## Check and deliver

Check that a new agent can understand the project without chat history, that no uncertain fact became a requirement, and that the current task is consistent with the current phase. Return requirements and constitution when ready; otherwise return confirmed understanding and the smallest useful set of questions. Include a concise list of remaining decisions. Never imply that a planning artifact is a working application.
