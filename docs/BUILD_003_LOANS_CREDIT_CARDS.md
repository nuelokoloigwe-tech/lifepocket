# Build 003 — Loans & Credit Cards

## Scope
- Add manually maintained loan and credit-card records.
- Store provider, current balance, APR, monthly repayment and next payment date.
- Credit cards additionally store credit limit and minimum payment.
- Loans additionally store original amount and expected end date.
- Calculate combined outstanding debt, monthly repayment commitments, available credit and credit utilisation.
- Record repayments, reduce the manually tracked balance, and retain a dated repayment history.
- Persist records in browser localStorage.

## Limitations
- No bank connection or automatic balance refresh.
- No interest accrual, amortisation schedule, payoff-date prediction or financial advice.
- After interest, fees or new borrowing, users must update the balance to match their lender statement.
- Repayment recording currently treats the entered amount as a direct reduction in balance; it does not split principal and interest.
