# Build 005 — Debt register visibility fix

- Replaced the compact View dropdown with two always-visible tabs: Credit Cards and Loans.
- Each tab displays its record count and selected register label.
- Loans is a first-class view; when no loans exist, the empty state prompts the user to add a row.
- Existing `lp-debts` localStorage records and Build 004 data structure are preserved.
- No bank integration is included.
