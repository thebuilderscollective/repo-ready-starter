# How we judge whether it works

Owner: [name]
Last reviewed: [date]
Status: evaluation plan only; no evaluation has been run.

## What this file holds
Record representative inputs or scenarios, expected behaviour, pass/fail
criteria, and observed results. Link each group of cases to its feature PRD.
Keep executable checks and datasets in an evals/ folder when you have them;
this Markdown file explains what they measure and how to run them.

## Example cases for the confirmation feature
Related plan: [PRD 002](prds/002-email-confirmation.md)

| Case | Expected behaviour | Result |
| --- | --- | --- |
| Stored signup, email service available | Send one accurate confirmation | Not run |
| Retry of the same signup event | Do not send duplicate confirmations | Not run |
| Email service unavailable | Record failure and allow a controlled retry | Not run |
| Course date has not been set | Do not invent a date or guarantee a seat | Not run |

## When the product uses AI
Include ordinary requests, ambiguous requests, missing information, and failures
you have seen. Define what a good answer or safe fallback looks like. For
variable outputs, record the rubric, model/prompt version, and number of runs.
Use repeatable cases; do not claim one successful demo proves reliability.

## Run record
- Date and product version: [fill in]
- Command or manual procedure: [verified steps, or not configured]
- Dataset or case version: [link]
- Results and failures: [evidence; never mark unrun checks as passed]
- Decision: [ship, fix, or investigate, with a reason]
