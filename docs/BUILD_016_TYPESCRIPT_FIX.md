# Build 016 — Loans & Cards TypeScript fix

- Usage now uses the numeric `limitValue` and `utilisedValue` variables.
- Removes the unused-variable TS6133 errors.
- Avoids arithmetic and comparison operations on `string | number` fields.
- Preserves select-on-focus and empty-to-zero-on-blur editing behaviour.
- Preserves Loans & Cards delete actions and all earlier Build 015 features.
