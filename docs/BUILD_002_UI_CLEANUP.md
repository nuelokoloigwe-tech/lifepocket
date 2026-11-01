# Build 002 UI cleanup — Payment actions

## Decision
Payment rows use a view-first interaction pattern. Permanent edit and delete icons have been removed from the bill list.

## Behaviour
- A single contextual three-dot control appears on each payment row.
- Selecting it reveals Edit payment and Delete payment actions.
- Edit opens the existing payment form.
- Delete retains the existing confirmation prompt.
- Mark paid remains a direct, prominent status action.
- The existing payment data and local persistence behaviour are unchanged.

## Acceptance criteria
- No permanent pencil or trash icons appear on payment rows.
- Each payment row has one accessible More options control.
- Edit and delete remain available from the contextual menu.
- Menu closes when an action is selected.
- Desktop and mobile layouts remain usable.
