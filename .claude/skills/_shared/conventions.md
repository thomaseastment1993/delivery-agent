# Shared Conventions

## RAG
- **Green**: on track; no intervention needed.
- **Amber**: at risk; recovery actions in place, may breach tolerance.
- **Red**: off track; breached tolerance, escalation needed.

## Scoring (risks)
Probability 1-5 x Impact 1-5 = Score. 1-6 Low, 8-12 Medium, 15-25 High.

## Issue severity
Critical / High / Medium / Low, with an owner and target date.

## IDs
Risks `R-001`, Issues `I-001`, Actions `A-001`, Benefits `B-001`, Decisions `D-001`, Dependencies `DEP-001`, Assumptions `AS-001`.

## Dates and money
ISO dates (YYYY-MM-DD). State currency explicitly; figures in thousands unless stated.

## Output formats
Every run of the areas below produces a deliverable file in addition to updating the markdown source of truth in `project-data/`.

| Area | Format | File |
|---|---|---|
| Status updates (weekly status, steering packs, exec summaries) | PowerPoint `.pptx` | `project-data/previous_outputs/YYYY-MM-DD-status.pptx` |
| Finance (budget, actuals, forecast, variance) | Excel `.xlsx` | `project-data/previous_outputs/YYYY-MM-DD-finance.xlsx` |
| Risks | Excel `.xlsx` | `project-data/previous_outputs/YYYY-MM-DD-risks.xlsx` |
| Issues | Excel `.xlsx` | `project-data/previous_outputs/YYYY-MM-DD-issues.xlsx` |

- Use the `anthropic-skills:pptx` skill to build `.pptx` files and `anthropic-skills:xlsx` for `.xlsx` files.
- Content comes only from `project-data/`; the deliverable must match the markdown. Never add figures that are not in the source.
- Include the as-at date, currency/units and RAG per conventions above. Flag assumptions and data gaps on the deliverable.
- Never overwrite an earlier output; add `-v2` if the same date is re-run. Keep history.
- If a file cannot be generated (tool or library unavailable), say so, still update the markdown, and do not claim an output exists.
- Benefits and RAID items not listed above (assumptions, dependencies) stay markdown only unless the user asks otherwise.
