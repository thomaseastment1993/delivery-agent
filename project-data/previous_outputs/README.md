# previous_outputs

Generated deliverables, kept as a dated history. See "Output formats" in `.claude/skills/_shared/conventions.md`.

- Status updates -> `.pptx`
- Finance, risks, issues -> `.xlsx`
- Naming: `YYYY-MM-DD-<topic>.<ext>`, e.g. `2026-11-24-status.pptx`, `2026-11-24-finance.xlsx`, `2026-11-24-risks.xlsx`, `2026-11-24-issues.xlsx`
- Never overwrite an earlier file; a re-run on the same date gets a suffix (`-v2`).
- These are snapshots. The markdown files in `project-data/` stay the source of truth.
- Contain client data: check before committing (see `.gitignore`).
