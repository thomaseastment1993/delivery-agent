---
name: weekly-status-report
description: Generate the weekly status report with RAG and key messages. Use for weekly reporting or steering packs.
---

# weekly-status-report

## Purpose
Repeatable, honest status reporting.

## When to use
- End of each reporting period

## Inputs
- Latest data in `project-data/`

## Process
1. Pull progress, milestones, RAID, finance, benefits.
2. Set RAG per dimension and overall.
3. Write key messages, asks and next steps.

## Output
`project-data/status/YYYY-MM-DD-status.md` (source of truth) and a PowerPoint `project-data/previous_outputs/YYYY-MM-DD-status.pptx`. Also produce the deliverable per "Output formats" in `../_shared/conventions.md`.

## References
Follow `../_shared/conventions.md`. Add supporting material to `references/`.
