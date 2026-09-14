# Agent Skills

Reusable workflows for coding and productivity agents. Maintained by [Zoy0707](https://github.com/Zoy0707).

## Choose a skill

1. [Master Prompt Builder](master-prompt-builder/): clarify a software idea and create a project constitution.
2. [Cover Letter Writer](cover-letter-writer/): write a concise application letter grounded in real experience.
3. [Personal ClickUp PM](personal-clickup-pm/): review personal tasks and identify useful next actions.
4. [Token Budget Guard](token-budget-guard/): notice costly inspection patterns and choose narrower tool requests.
5. [Writing Voice](writing-voice/): revise prose using confirmed preferences and learn only from authorized evidence.

## Install

Clone this repository into a temporary directory, then copy the skill folder you want into your agent's personal skill directory. For Codex, this is usually `~/.codex/skills/`. Back up an existing folder before replacing it. Start a new task so the skill can be discovered.

For another agent, use its documented installation method. These are text instructions; available tools depend on the host.

## Use

Ask the agent to use a skill by name and provide the task inputs. Each folder has a short guide and a realistic invocation example.

## Privacy and limits

Keep resumes, private profiles, customer records, credentials, and workspace identifiers in your own environment. Do not commit them to this repository. Actual writing profiles are not included.

Skills guide behavior but do not guarantee outcomes. ClickUp requires a connected account. Token warnings are estimates unless a host provides a suitable meter. See [validation](VALIDATION.md) for the scope of checks.
