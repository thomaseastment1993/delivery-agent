# Delivery Agent

Delivery-lead toolkit for programme/project delivery. See README.md.

## Structure
- `.claude/agents/`, `.claude/skills/`, `.claude/commands/`, `.claude/hooks/`
- `.claude/skills/_shared/conventions.md` — RAG, scoring and ID conventions; all agents and skills follow it
- `project-data/` — source of truth for project state; agents read and update it

## Rules
- Never invent data. If something is missing, flag it as an assumption or open question.
- Update `project-data/` files rather than only replying in chat.
- Keep client-confidential data out of commits (see .gitignore).
