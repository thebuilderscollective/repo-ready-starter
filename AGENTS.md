# Working agreements

## Start here
- Read README.md for setup and verified check commands.
- Inspect recent Git commits, git status, and the staged and unstaged diffs for context.
- Check untracked files too. Verify commit messages against the current code.
- Read the PRD named in the request and any linked issue or pull request.
- Use docs/product.md for the user, scope, and definition of success.
- For interface work, read DESIGN.md; for system changes, read docs/architecture.md.
- For contributions, read CONTRIBUTING.md.
- For feature work, read the relevant plan in docs/prds/ and checks in docs/evals.md.
- For application work, read app/AGENTS.md; for billing, also read
  app/billing/AGENTS.md. These paths are relative to the repository root.

## While working
- Make the smallest change that satisfies the agreed task.
- Keep files focused; split unrelated responsibilities when a file becomes hard to follow.
- Trace the existing flow before choosing where to edit.
- Add tests for changed behaviour under tests/ using the project's existing framework.
- State assumptions. Ask when a missing decision materially changes scope.
- Follow existing patterns. Explain before adding a new dependency.
- Keep credentials and customer data out of code, docs, and examples.
- Work on a branch from the latest main. Land changes through a pull request.
- Never force-push or rewrite published history.

## Before handing over
- Run the relevant checks documented in README.md. Never claim an unrun check passed.
- If no automated checks exist, describe the manual verification and its limits.
- Keep useful reasons and verification results in commit messages and pull requests.
- Record open questions in the relevant PRD, issue, or pull request.
- Record a consequential decision in docs/decisions/ with its reason.
- Update a rule only when the working agreement actually changes.

These are instructions, not access controls. Configure repository protections,
permissions, and checks separately where enforcement matters.
