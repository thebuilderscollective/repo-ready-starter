# Billing working agreements

Scope: app/billing/. Add these to the root and app/ guidance.
Illustrative rules for a future billing area; no payment integration exists yet.

- Validate prices and totals on the server; do not trust browser-supplied totals.
- Check rounding, failed payments, and duplicate payment events when affected.
- Use sandbox test data; keep payment credentials and customer data out of docs.

These rules guide implementation. They do not authorize real charges or refunds.
