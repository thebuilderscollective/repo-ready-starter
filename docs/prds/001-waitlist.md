# PRD 001: collect interest

Status: example / proposed, not implemented
Owner: [name]
Last reviewed: [date]
Product context: [product.md](../product.md)

## Problem and outcome
A visitor interested in a future course can leave an email address and see a
clear confirmation that their interest was recorded.

## Scope
One form with email validation, storage, and success/error states.
Accounts, payments, and confirmation emails are out of scope for this first step.

## Acceptance criteria
- A valid email is recorded once, including after a repeated submission.
- Invalid input gets a useful error message.
- A failed request preserves the input and allows a retry.
- Keyboard and narrow-screen use work.

## Decisions needed
Choose storage, consent wording, and retention before connecting a real service.

## Delivery and evaluation
Add executable acceptance checks under tests/ when the application exists.
Use [evals.md](../evals.md) for the evaluation format and record relevant cases.
A later feature can add [email confirmation](002-email-confirmation.md).
