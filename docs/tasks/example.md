# Example task: collect interest

Status: example only; replace before implementation.
Feature plan: [PRD 001](../prds/001-waitlist.md).

## Outcome
A visitor can leave an email address and see a confirmation.

## In scope
One email field, validation, a submit action, and success/error messages.

## Out of scope
Accounts, payments, and a full email marketing platform.

## Acceptance checks
- A valid email is accepted and stored once.
- Invalid input gets a useful error message.
- A failed request preserves the input and offers a retry.
- The form works with a keyboard and on a narrow screen.

## Decisions needed
Where should email addresses be stored, and what consent text is required?
Resolve these before connecting a real service.
