# Your project, ready for the next conversation

A small documentation starter from The Builder Course. No framework, no dependencies, no ceremonial folders. Use it for an app, a prototype, or an agent workflow.

## Make it yours in 10 minutes

1. On GitHub, choose **Use this template → Create a new repository**. Or download the ZIP and copy the files into your project folder.
2. Replace the bracketed prompts in this README and `docs/product.md` with real answers. Delete what you do not need.
3. Fill in verified setup and check commands below. There is no runnable application in this template yet.
4. Review `AGENTS.md`. `CLAUDE.md` imports it, so shared rules have one home.
5. Open your coding agent in this folder. Ask it to read `AGENTS.md`, `docs/README.md`, and `docs/handoff.md`, then summarize the next step.

## What we are building

[Product name] helps [specific person] do [specific job].

## Run it

- Requirements: [tools and versions; none required for this docs-only starter]
- Install: [verified command, or not applicable]
- Start locally: [verified command, or not applicable]
- Check changes: [verified command, or describe a manual check]
- Expected result: [what success looks like]

Do not invent commands. Replace these prompts when you add the application.

## Find your bearings

- `AGENTS.md`: shared working rules for coding agents.
- `CLAUDE.md`: Claude Code entry point importing the shared rules.
- [Docs index](docs/README.md): what to read for each kind of task.
- [Product brief](docs/product.md): user, problem, scope, success.
- [Current handoff](docs/handoff.md): where the work stands and what comes next.
- [Decisions](docs/decisions/README.md): why we chose something.
- [Example task](docs/tasks/example.md): one small, checkable piece of work.

Keep credentials out of these files. `.env.example` lists variable names with empty values; `.gitignore` excludes local secrets. You still need to review what you commit.

## The next conversation

Open the same project folder (or a checkout containing your latest saved files) and say:

> Read AGENTS.md, docs/README.md, and docs/handoff.md. Summarize the current state and proposed next step. Check the actual files before making changes.

Before leaving a session, update the handoff. A new chat can read a file; it cannot reconstruct an unsaved decision.

## About this starter

By Rajat, for [The Builder Course](https://www.thebuildercourse.com). Adapt the structure as the project grows. Names will change; keeping intent, rules, decisions, and current state findable is the principle.

Instruction behavior checked 22 September 2026: [Codex](https://learn.chatgpt.com/docs/agent-configuration/agents-md) · [Claude Code](https://code.claude.com/docs/en/memory).
