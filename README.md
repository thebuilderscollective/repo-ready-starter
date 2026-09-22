# Your project, ready for the next conversation

A small documentation starter from The Builder Course. No framework or application dependencies. Start with the essentials; keep the optional files when they help. Use it for an app, a prototype, or an agent workflow.

## Make it yours in 10 minutes

1. On GitHub, choose **Use this template → Create a new repository**. Or download the ZIP and copy the files into your project folder.
2. Replace the bracketed prompts in this README and `docs/product.md` with real answers. Delete files you do not need and repair links to them.
3. Fill in verified setup and check commands below. There is no runnable application in this template yet.
4. Review `AGENTS.md`. `CLAUDE.md` imports it, so shared rules have one home.
5. Open your coding agent in this folder. Ask it to read `README.md`, `AGENTS.md`, `docs/product.md`, and `docs/handoff.md`, then summarize the next step.

## What we are building

[Product name] helps [specific person] do [specific job].

## Run it

- Requirements: [tools and versions; none required for this docs-only starter]
- Install: [verified command, or not applicable]
- Start locally: [verified command, or not applicable]
- Check changes: [verified command, or describe a manual check]
- Expected result: [what success looks like]

Do not invent commands. Replace these prompts when you add the application.

## Choose what you need

Start with README.md, AGENTS.md, docs/product.md, and docs/handoff.md.
Keep CLAUDE.md if you use Claude Code. The rest demonstrates how to grow:

- [CONTRIBUTING.md](CONTRIBUTING.md): how teammates propose and verify changes.
- [DESIGN.md](DESIGN.md): visual and interaction conventions.
- [Feature PRDs](docs/prds/README.md): one plan per substantial feature or change.
- [Evaluations](docs/evals.md): scenarios, expected behaviour, and results.
- [Architecture](docs/architecture.md): components, data flow, and boundaries.
- [CHANGELOG.md](CHANGELOG.md): changes people using the product care about.
- [Release runbook](docs/runbooks/release.md): prerequisites, steps, checks, recovery.

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

`.agents/skills/write-handoff/SKILL.md` is a small optional Codex skill: a reusable
recipe for updating the handoff. Try `$write-handoff` in a Codex session where
this repository's skills are available. Its name and description help discovery;
the full recipe loads when selected. The leading dot is a hidden-folder convention.

AGENTS.md holds working rules; `.agents/skills/` packages reusable workflows.
Putting arbitrary Markdown in `.agents/` does not make it load automatically.
Claude Code documents `.claude/skills/` for project skills; move or link this skill
there if needed, and verify discovery in your tool. The CLAUDE.md import shares
instructions, not skill installation.

## Keeping the docs current

Keep the files you actually need. No one gets extra points for empty files.
Each extra file adds maintenance: give it an owner, review it when the related
behaviour changes, and remove or archive it when it stops helping.

Keep one living docs/product.md for the whole product. Write feature-specific
PRDs under docs/prds/ as the product evolves. Use a separate PRD for a substantial change; a small fix can stay in a task. docs/evals.md records how you assess the
results. The two example PRDs show an initial waitlist and a later email feature.

## Find your bearings

- `AGENTS.md`: shared working rules for coding agents.
- `CLAUDE.md`: Claude Code entry point importing the shared rules.
- [Docs index](docs/README.md): an optional map of docs/, separate from this root README.
- [Product brief](docs/product.md): user, problem, scope, success.
- [Current handoff](docs/handoff.md): where the work stands and what comes next.
- [Decisions](docs/decisions/README.md): why we chose something.
- [Example task](docs/tasks/example.md): one small, checkable piece of work.

Keep credentials out of these files. `.env.example` lists variable names with empty values; `.gitignore` excludes local secrets. You still need to review what you commit.

## The next conversation

Open the same project folder (or a checkout containing your latest saved files) and say:

> Read README.md, AGENTS.md, docs/product.md, and docs/handoff.md. Summarize the current state and proposed next step. Check the actual files before making changes.

Before leaving a session, update the handoff. A new chat can read a file; it cannot reconstruct an unsaved decision.

## About this starter

By Rajat, for [The Builder Course](https://www.thebuildercourse.com). Adapt the structure as the project grows. Names will change; keeping intent, rules, decisions, and current state findable is the principle.

Instruction behavior checked 22 September 2026: [Codex](https://learn.chatgpt.com/docs/agent-configuration/agents-md) · [Claude Code](https://code.claude.com/docs/en/memory).

Skills references: [Codex](https://learn.chatgpt.com/docs/build-skills) · [Claude Code](https://code.claude.com/docs/en/skills).
