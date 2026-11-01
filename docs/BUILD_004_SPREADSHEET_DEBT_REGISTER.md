# Build 004 — Spreadsheet-style Loans & Credit Cards

## What changed
- Replaced the separate debt-entry form and account cards with editable tables.
- Added Credit Cards and Loans views.
- Credit Cards columns: name, limit, utilised amount, available credit and utilisation percentage.
- Loans columns: name, original amount, outstanding balance, monthly repayment, APR and next payment date.
- Added an inline new row action for each view.
- Totals and credit utilisation recalculate as cells are edited.
- Existing `lp-debts` localStorage records are retained; existing balances are treated as amounts owed/utilised.

## Notes
- Available credit = credit limit − utilised amount, floored at zero.
- Utilisation = utilised amount ÷ total credit limit.
- Loan balances and APRs remain manually maintained. No interest accrual or payoff forecast is calculated.
- Data remains in browser localStorage on this device.
