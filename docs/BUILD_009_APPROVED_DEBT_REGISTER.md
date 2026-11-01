# Build 009 — Approved debt register

## What changed
- Replaced the previous multi-field debt screen with a category-driven register.
- Categories: Car Finance, Personal Loan, Mortgage, Student Loan, Business Loan, Credit Card and Other Loan.
- Exact columns: Item, Limit (£), Utilised (£), Balance (£), Usage.
- Balance is calculated as `max(0, Limit - Utilised)`.
- Usage is calculated as `Utilised / Limit × 100` (0% when Limit is zero).
- Users can add, edit and delete rows.
- Data is saved locally in the browser using `lp-debt-register`.

## Deliberately excluded
APR, interest rate, provider, monthly repayment, due date and other extra fields.
