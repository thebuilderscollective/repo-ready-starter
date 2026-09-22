---
name: write-handoff
description: Update docs/handoff.md when the user asks to wrap up a session or prepare a handoff for the next conversation.
---

# Write a useful handoff

Use the repository's docs/handoff.md as the output format.

Review the current handoff and the changes available in this session. Record:
- the date, goal, and current branch or commit when available;
- what changed, with links or paths to the relevant files;
- checks actually run, their results, and anything not verified;
- unresolved issues and one concrete next step.

Replace stale current-state notes rather than appending an endless diary.
Keep important historical reasoning in docs/decisions/ and link to it.
Do not invent checks, results, or details from earlier chats you cannot access.
Keep secrets and customer data out. Save the handoff locally; this workflow
alone does not authorize commits, pushes, messages, or deployments.
