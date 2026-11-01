# Build 002 — Personal Life & Finance

## Scope
Build 002 keeps the existing premium interface and expands everyday organisation without bank connectivity.

### Included
- Existing overview, recurring bill reminders, payment history and calendar
- Task management
- Shopping Manager: add, categorise, complete and remove shopping items
- Document Wallet index: add a file to record its name, size and date; remove an entry
- Local browser persistence for demo records

### Explicit exclusions
- Bank connections, bank balances, bank statement imports, transaction feeds and Open Banking
- Cloud authentication, synchronisation and remote storage
- Automated push/email notifications
- AI financial or personal assistant

### Known limitations
- All demo data is stored in browser localStorage on one device/browser.
- Document Wallet stores metadata only, not the uploaded file contents.
- Reminders are displayed in the application; this build does not send notifications in the background.
- Financial summaries relate to manually entered bill reminders, not a complete ledger or bank account balance.

## Acceptance checks
1. Add a recurring payment and verify it appears in the payment list/calendar.
2. Mark a recurring payment paid and verify history is updated and its due date advances.
3. Add a task, complete it and refresh the browser.
4. Add a shopping item, categorise it, mark it complete and refresh.
5. Add a document entry and verify its metadata appears; remove the entry.
6. Confirm no bank connection, balance or statement-import feature is presented.
