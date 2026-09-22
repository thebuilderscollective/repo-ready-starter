# Your project, ready for the next conversation

A small documentation starter from The Builder Course. No application framework. The optional test placeholders use Node.js. Start with the essentials; keep the optional files when they help. Use it for an app, a prototype, or an agent workflow.

## Make it yours in 10 minutes

1. On GitHub, choose **Use this template → Create a new repository**. Or download the ZIP and copy the files into your project folder.
2. Replace the bracketed prompts in this README and `docs/product.md` with real answers. Delete files you do not need and repair links to them.
3. Fill in verified setup and check commands below. There is no runnable application in this template yet.
4. Review `AGENTS.md`. `CLAUDE.md` imports it, so shared rules have one home.
5. Open your coding agent in this folder. Ask it to read `README.md`, `AGENTS.md`, and `docs/product.md`, then inspect recent Git commits and the current diff before proposing a next step.

## What we are building

[Product name] helps [specific person] do [specific job].

## Run it

- Requirements: [tools and versions; Node.js only if running the test placeholders]
- Install: [verified command, or not applicable]
- Start locally: [verified command, or not applicable]
- Check changes: [verified command, or describe a manual check]
- Expected result: [what success looks like]

Do not invent commands. Replace these prompts when you add the application.

## Choose what you need

Start with README.md, AGENTS.md, and docs/product.md.
Keep CLAUDE.md if you use Claude Code. The rest demonstrates how to grow:

- [CONTRIBUTING.md](CONTRIBUTING.md): how teammates propose and verify changes.
- [DESIGN.md](DESIGN.md): visual and interaction conventions.
- Feature PRDs: [waitlist](docs/prds/001-waitlist.md) and [email confirmation](docs/prds/002-email-confirmation.md). Both are proposed examples.
- [Evaluations](docs/evals.md): scenarios, expected behaviour, and results.
- [Architecture](docs/architecture.md): components, data flow, and boundaries.
- [CHANGELOG.md](CHANGELOG.md): changes people using the product care about.
- [Release runbook](docs/runbooks/release.md): prerequisites, steps, checks, recovery.
- [tests/waitlist.test.mjs](tests/waitlist.test.mjs): TODO examples to replace with real application tests.
- [.gitlab-ci.yml](.gitlab-ci.yml): a disabled GitLab CI example, with the GitHub equivalent explained inside.

Delete optional examples you do not need. A folder structure is not homework.

## Try the instruction hierarchy

There are three real levels: `AGENTS.md` -> `app/AGENTS.md` ->
`app/billing/AGENTS.md`. The root sets shared agreements; app adds interface and
flow checks; billing adds money-specific validation and failure cases. The app/
folder is an instructional example, not a runnable application.

For Codex, start in `app/billing/` and ask which instruction files loaded.
Its startup discovery walks from the repo root to the working directory.
From the root, explicitly ask it to read the nested files for that task.

Each level has a CLAUDE.md containing just `@AGENTS.md`, importing the neighbouring AGENTS.md.
Claude Code loads ancestor guidance at startup and nested guidance as it reads
files in those folders. Keep these additive rules consistent; do not rely on
conflicting instructions being resolved the same way across tools.

## What is .agents/ doing here?

`.agents/skills/grill-me/SKILL.md` is a labelled placeholder showing where a
skill belongs. It is not an upstream skill installation. Replace it with the
version you choose to use. SKILL.md contains a name, description, and instructions.

The leading dot is a hidden-folder convention. Codex uses .agents/skills/;
Claude Code documents .claude/skills/ for project skills. The CLAUDE.md import
shares working rules; it does not install skills across tools.

## Tests and CI

Run `node --test tests/*.test.mjs` to see the three TODO test placeholders.
They make no assertions and provide no coverage. Replace them with tests of
your actual application, using the test framework appropriate to your project.

The GitLab CI example is disabled until real checks exist. On GitHub, create a
workflow such as .github/workflows/ci.yml using GitHub Actions syntax. Moving or
renaming a GitLab file does not convert it. CI runs checks; it does not decide
whether those checks are enough.

## Keeping the docs current

Keep the files you actually need. No one gets extra points for empty files.
Each extra file adds maintenance: give it an owner, review it when the related
behaviour changes, and remove or archive it when it stops helping.

Keep one living docs/product.md for the whole product. Write feature-specific
PRDs under docs/prds/ as the product evolves. Use a separate PRD for a substantial change; a small fix can be described in its issue or pull request. docs/evals.md records how you assess the
results. The two example PRDs show an initial waitlist and a later email feature.

## Find your bearings

- `AGENTS.md`: shared working rules for coding agents.
- `CLAUDE.md`: Claude Code entry point importing the shared rules.
- [Product brief](docs/product.md): user, problem, scope, success.
- [Decision example](docs/decisions/001-shared-agent-rules.md): why we chose something.

The root README is the document map. The docs/ and prds/ folders do not need their own README files.

Keep credentials out of these files. `.env.example` lists variable names with empty values; `.gitignore` excludes local secrets. You still need to review what you commit.

## The next conversation

Open the same project folder (or a checkout containing your latest saved files) and say:

> Work on docs/prds/002-email-confirmation.md. Follow the project instructions and show me your plan before editing.

AGENTS.md routes the next session through recent commits and the current working
tree, then the requested PRD and relevant project files. For application changes,
app/AGENTS.md supplies local rules; README.md names check commands and
CONTRIBUTING.md explains the review process. Keep files focused and add behaviour
tests in tests/ as the application grows.

Use meaningful commits and pull requests to record completed changes, their
reasons, and verification results. Put open questions in the relevant PRD,
issue, or pull request. A fresh checkout cannot see your uncommitted files or
recover decisions left only in chat.

## About this starter

By Rajat, for [The Builder Course](https://www.thebuildercourse.com). Adapt the structure as the project grows. Names will change; keeping intent, rules, decisions, and current state findable is the principle.

Instruction behavior checked 22 September 2026: [Codex](https://learn.chatgpt.com/docs/agent-configuration/agents-md) · [Claude Code](https://code.claude.com/docs/en/memory).

Skills references: [Codex](https://learn.chatgpt.com/docs/build-skills) · [Claude Code](https://code.claude.com/docs/en/skills).
