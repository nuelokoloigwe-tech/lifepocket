# Build 002 — Reversible payment marking

## Behaviour
- Marking a bill paid records a payment-history entry including the original due date.
- Recurring bills advance to their next due date as before.
- During the same calendar month in which a payment was recorded, the payment-history row offers **Undo payment**.
- Undo requires confirmation, removes the history entry, restores the original due date and returns the bill to outstanding.
- Undo is unavailable after the calendar month changes.
- Monthly history totals recalculate from the remaining payment records.

## Acceptance criteria
1. Mark a monthly recurring bill paid; its next due date advances.
2. Undo it during the same month; the history record disappears and the original due date is restored.
3. Confirm the monthly total decreases after undo.
4. One-off payments return to unpaid when undone.
5. A payment recorded in a previous month has no undo action.

## Data compatibility
The `dueBefore` field is optional so existing locally stored payment-history records remain readable. New records store it to support accurate restoration.
