# The map

Read only what the task needs. Most documents here are ordinary Markdown;
AGENTS.md routes work here rather than assuming every document loads itself.

| Your question | Read |
| --- | --- |
| Who is this for, and what is in scope? | [product.md](product.md) |
| Where did we stop? | [handoff.md](handoff.md) |
| How do the parts connect? | [architecture.md](architecture.md) |
| How should the interface feel? | [DESIGN.md](../DESIGN.md) |
| How do I contribute? | [CONTRIBUTING.md](../CONTRIBUTING.md) |
| Why did we choose this? | [decisions/](decisions/README.md) |
| What is the next small piece of work? | [tasks/example.md](tasks/example.md) |
| How would we release and recover? | [runbooks/release.md](runbooks/release.md) |
| What changed for users? | [CHANGELOG.md](../CHANGELOG.md) |

## Rules for this area

[AGENTS.md](AGENTS.md) adds documentation-specific guidance to the root rules.
[runbooks/AGENTS.md](runbooks/AGENTS.md) adds operational-document guidance one
level deeper. Matching CLAUDE.md imports expose these rules to Claude Code.

Each fact should have one authoritative home. Link to it elsewhere. Update
current guidance with the change it describes; mark replaced decisions as
superseded. Archive finished task notes when they obscure current work.

The extra documents are starter examples. Keep only the ones you need.
