# Agent Skills

Small, reusable workflows for coding and productivity agents. Maintained by [Zoy0707](https://github.com/Zoy0707).

| Skill | Use it for |
| --- | --- |
| [Master Prompt Builder](master-prompt-builder/) | Turn a software idea into requirements and a coding-agent project constitution. |
| [Cover Letter Writer](cover-letter-writer/) | Write a short application letter grounded in real experience. |
| [Personal ClickUp PM](personal-clickup-pm/) | Review and organize personal tasks without overcomplicating the workspace. |

## Install

Clone this repository into a temporary directory, then copy the skill folder you want into your Codex personal skills directory (usually `~/.codex/skills/`). Back up any existing folder with the same name before replacing it. Start a new task so the installed skill can be discovered.

For another agent, use its documented skill installation method. These workflows are text instructions; tool availability depends on your host.

## Use

Ask your agent to use the skill by name:

```text
Use master-prompt-builder to clarify this idea: a shared reading list for a book club.
Use cover-letter-writer with the resume and job description below. Ask me for missing evidence.
Use personal-clickup-pm to review my personal Space [SPACE ID]. Do not change tasks yet.
```

## Privacy and limitations

Supply private inputs in your own environment. Do not commit resumes, story banks, customer records, credentials, or workspace IDs to this repository. No personal examples or private repository history are included.

These skills guide an agent; they do not guarantee outcomes. ClickUp requires a connected account. Skill-level scenario checks are not live integration tests. See [validation](VALIDATION.md).
