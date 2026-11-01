# Build 002 – Shopping Lists and Monthly Payment History

## Shopping lists
- Users can create multiple named shopping lists for separate market trips, shops or occasions.
- Each list has its own items and completion state.
- Items can be categorised as Groceries, Household, Personal or Other.
- Users can filter the active list by category, add items, mark items complete, delete items and clear completed items.
- Existing shopping items without a list identifier remain visible in the default “Market run” list.
- Shopping lists and items are stored in browser localStorage in this prototype.

## Payments
- The Money page has a category filter for payment reminders.
- The payment summary shows the amount paid in the current month.
- Monthly payment history can be browsed by month and shows the total and individual payment records for the selected month.
- A history entry is created when a user marks a payment as paid.
- Payment records remain local to the browser in this prototype.

## Limitations
- No bank connections or bank statement imports are included.
- Data is stored locally in the current browser and is not synchronised across devices.
- Historical payment records reflect payments recorded in LifePocket after this feature is available; they do not reconstruct payments from before the app was used.
