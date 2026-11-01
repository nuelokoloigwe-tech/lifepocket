# Payment management update

Payment reminders are user-manageable rather than fixed display-only values.

## Supported actions
- Add a payment reminder.
- Edit the title, category, amount, due date and frequency of an existing reminder.
- Delete a reminder after confirmation.
- Mark a reminder as paid using the existing payment-history workflow.

Changes are saved to this browser's localStorage under `lp-payments` and update the dashboard, Money view and calendar from the same payment state.

## Sample data
The initial payment list remains sample data for first-time users. Users can edit or delete these entries. Existing saved `lp-payments` data is retained when the app is updated; the new build does not overwrite it.

## Limitations
Data remains local to the browser/device. There is no account sync or cloud backup in this build.
