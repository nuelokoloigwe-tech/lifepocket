# Build 011 — Dedicated Income page and monthly income history

## Changes
- Added Income as a dedicated workspace navigation page, separate from Money.
- Kept Money focused on Payments; the default Payments view remains unchanged.
- New income sources start with a blank editable name and a helpful example placeholder instead of “New income source”.
- Added a monthly income receipt form for recording the source, category, amount and date actually received.
- Monthly receipts are saved separately from expected income sources in browser local storage (`lp-income-entries`).
- Added a month selector, monthly total and receipt history. Entries are grouped by their received date, so October records remain available when November begins.
- Preserved the existing income-source data key (`lp-income`) and existing payment/debt data keys.

## Important behaviour
The source register describes expected income. The monthly receipt history records actual money received. Recording a receipt does not automatically change or delete the expected source. Records are stored on the current device/browser; this build does not sync them to an account or cloud database.

## Verification
- Source archive structure and ZIP integrity checked.
- A production build could not be verified in this environment because dependencies were not installed; `npm install` timed out. Run `npm.cmd install` and `npm.cmd run build` in PowerShell on the user's machine before deployment.
