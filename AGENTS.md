# Working agreements

## Start here
- Read README.md for setup and verified check commands.
- Read docs/README.md to find task-specific context.
- Read docs/handoff.md; verify its claims against the current files.
- Use docs/product.md for the user, scope, and definition of success.

## While working
- Make the smallest change that satisfies the agreed task.
- State assumptions. Ask when a missing decision materially changes scope.
- Follow existing patterns. Explain before adding a new dependency.
- Keep credentials and customer data out of code, docs, and examples.
- Work on a branch from the latest main. Land changes through a pull request.
- Never force-push or rewrite published history.

## Before handing over
- Run the relevant checks documented in README.md. Never claim an unrun check passed.
- If no automated checks exist, describe the manual verification and its limits.
- Update docs/handoff.md with changes, evidence, open issues, and the next step.
- Record a consequential decision in docs/decisions/ with its reason.
- Update a rule only when the working agreement actually changes.

These are instructions, not access controls. Configure repository protections,
permissions, and checks separately where enforcement matters.
