# Delivery Agent

Delivery-lead toolkit for programme/project delivery. See README.md.

## Structure
- `.claude/agents/`, `.claude/skills/`, `.claude/commands/`, `.claude/hooks/`
- `.claude/skills/_shared/conventions.md` — RAG, scoring and ID conventions; all agents and skills follow it
- `project-data/` — source of truth for project state; agents read and update it
- `project-data/context-sources.md` — index of supporting external context

## Rules
- Never invent data. If something is missing, flag it as an assumption or open question.
- Update `project-data/` files rather than only replying in chat.
- Consult `project-data/context-sources.md` when relevant. Follow links only through tools and permissions available in the current environment; a listed URL does not guarantee access. If a source is inaccessible, state that explicitly rather than inferring its contents.
- Treat linked sources as supporting context, not as a replacement for managed project records. Flag conflicting information with its source and date; do not silently resolve the conflict.
- Keep client-confidential data out of commits (see .gitignore).
