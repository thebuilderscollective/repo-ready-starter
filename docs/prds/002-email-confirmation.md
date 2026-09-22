# PRD 002: confirm interest by email

Status: example / proposed, not implemented
Owner: [name]
Last reviewed: [date]
Depends on: [PRD 001](001-waitlist.md)
Product context: [product.md](../product.md)

## Problem and outcome
After a successful signup, the visitor gets an email confirming that their
interest was recorded. It must not imply a paid booking or guaranteed seat.

## Scope
One confirmation message after storage succeeds, plus delivery-failure handling.
Marketing campaigns and payment receipts are out of scope.

## Acceptance criteria
- Successful storage triggers one confirmation, even if the request is retried.
- A delivery failure is observable and can be retried without duplicate signups.
- The message describes the actual signup state and invents no course dates.

## Decisions needed
Choose the email provider, approved copy, sender, and retry policy.

## After shipping
Mark this PRD shipped. Update product.md to describe the available confirmation
flow, architecture.md for the provider, and evals.md for the checks performed.
