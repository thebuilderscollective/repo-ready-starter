# Decision example: share agent rules

Status: illustrative example
Date: [date]

## Context
Codex and Claude Code use different instruction filenames. Two copies of the
same working rules can drift when only one gets updated.

## Choice
Keep the shared rules in AGENTS.md. Let the neighbouring CLAUDE.md import them
with @AGENTS.md, as shown in this starter.

## Tradeoff
One place to edit shared rules, with tool-specific loading behaviour still to
verify. Separate instructions may be needed when the tools have different jobs.

## Revisit when
The team's tools or their instruction-loading rules change.

Use a short record like this for decisions whose reasons would otherwise be
hard to recover. Link the relevant commit or pull request when available.
