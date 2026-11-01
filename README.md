# LifePocket — Build 004

A personal life-management prototype built with React, TypeScript and Vite.

## Run locally

1. Extract this folder.
2. Open the extracted `lifepocket-build-001` folder in VS Code.
3. In the terminal run:

   ```powershell
   npm.cmd install
   npm.cmd run dev
   ```

4. Open the local URL printed by Vite.

## Build 004
Loans & Cards now uses an editable spreadsheet-style register. Switch between Credit Cards and Loans, add a row, and type directly into the cells. Credit-card available credit and utilisation plus table totals are calculated automatically.

Data is stored locally in the browser. This is a prototype, not a cloud-synchronised or bank-connected service.


## Build 005 — Debt register visibility
The Loans and Credit Cards views are now exposed as clear, always-visible tabs. Select **Loans** to open the loan register, then use **Add loan** to create a row.


## Build 006 — Spreadsheet-style debt register
Credit Cards and Loans are separate registers with direct cell editing. Both include provider fields. Credit card available credit and utilisation are calculated automatically. Loan original amount, outstanding balance, monthly repayment, APR and next payment date are editable. Empty registers show an explicit Add first row action. Data is stored locally in this browser; no bank connection is used.


## Income register
The Money workspace now opens with an Income tab and a Payments tab. Income supports direct table entry for source, category, amount, frequency and next pay date. Monthly income is estimated from weekly, fortnightly, monthly, quarterly and annual amounts; one-off income is excluded. Entries are stored locally in the browser under `lp-income`. No sample personal income is preloaded.


## Build 009 — Approved debt register
The Loans & Cards area now uses a category dropdown and the approved five-column register: Item, Limit, Utilised, Balance and Usage. Balance and Usage are calculated automatically; changes persist in browser local storage under `lp-debt-register`.

Build 010 adjustment: the Money section opens on Payments by default to preserve the previous experience; Income remains available as a separate tab.
