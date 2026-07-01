# Dehumidifier

A systematic 9-pass protocol for detecting and eliminating AI-generated writing patterns — for use as a Claude Project skill (or adapted for any LLM writing workflow).

Named because it strips out the artificial moisture that makes AI prose feel bloated and stiff.

## What it does

Most AI writing "cleanup" just swaps one template for another — "Moreover" becomes "Picture this:" and it's still a tell. This skill runs nine distinct audit passes (title/opening, sentence structure, vocabulary, paragraph structure, logic, rhetorical devices, verbosity, fake-casual tells, and a final "human messiness" check) to catch patterns that survive a single editing pass.

## Usage modes

| Mode | Trigger phrase | What it does |
|---|---|---|
| Audit Only | "audit this for AI tells" | Flags every pattern found, quotes the offending phrase, no rewrite |
| Full Edit | "dehumidify this" / "humanize this" | Runs all 9 passes, produces a clean rewrite |
| Single Pass | "dehumidify [issue] only" | Targets one category (e.g. just vocabulary) |
| Score Report | "score this for AI tells" | 0–100 score with category breakdown |

## How to use

Drop `SKILL.md` into a Claude Project's custom skills folder, or paste its contents as a system/project instruction. Full setup instructions: https://support.claude.com/en/articles/12512138-using-skills-in-claude-ai

## Status

v1 — actively maintained, refined through real editing sessions rather than written top-down.
