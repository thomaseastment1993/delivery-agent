# Delivery Agent

A Claude Code project that acts as a **Delivery Lead**. A lead agent orchestrates five specialist sub-agents, supported by reusable skills.

| Agent | Responsibility |
|---|---|
| `delivery-lead` | Orchestrator: routes work, consolidates outputs, escalates |
| `risk-manager` | Identify, score, and track risks and mitigations |
| `issue-manager` | Log, triage, and drive issues to resolution |
| `status-reporter` | Produce RAG status reports and steering-committee packs |
| `benefit-realisation` | Define, baseline, and track benefits to realisation |
| `financial-manager` | Budget, actuals, forecast, and variance analysis |

## Structure
- `.claude/agents/`   one `.md` per agent (frontmatter + prompt)
- `.claude/skills/`   one folder per skill, each with `SKILL.md`; `_shared/` holds common conventions
- `.claude/commands/` slash commands (e.g. `/weekly-status`)
- `.claude/hooks/`    hook scripts, wired in `.claude/settings.json`
- `project-data/`     your project's working data (RAID, status, benefits, finance)

## Getting started
1. Fill in `project-data/project-charter.md`.
2. Open the folder in Claude Code and ask the delivery lead, e.g. "Run the weekly status cycle".
3. Add agents by copying `.claude/agents/_template-agent.md`; add skills by copying `.claude/skills/_template-skill`.

## Conventions
See `.claude/skills/_shared/conventions.md` (RAG definitions, scoring scales, ID formats).
