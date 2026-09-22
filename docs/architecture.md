# How the pieces connect

Status: planning template; no application is implemented yet.
Last reviewed: [date]

## The main journey
[Describe what happens from a user action to a result.]
Example only: visitor submits a form -> server checks it -> database stores it
-> email service sends a confirmation.

## Components and ownership
| Part | Responsibility | Where it lives |
| --- | --- | --- |
| [Interface] | [What the user sees and does] | [Folder] |
| [Server] | [Validation and business rules] | [Folder] |
| [Storage] | [What persists] | [Service or folder] |

## Boundaries
- External services: [what we rely on and why]
- Sensitive data: [what exists, where it lives, and who can access it]
- Failure modes: [what happens when a dependency is unavailable]

## Related decisions
[Link to decisions/ records for the reasons behind these choices.]

Describe today's system. Put speculative plans in a clearly marked section.
