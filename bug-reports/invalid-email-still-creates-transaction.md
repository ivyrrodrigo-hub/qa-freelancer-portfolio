# Bug Report: Invalid Email Validation Appears but Transaction Still Gets Created

## Summary
The UI shows an invalid email error, but the payment transaction is still submitted to the backend.

## Environment
- Platform: Web
- Browser: Chrome
- Module: Subscription / Credit Card Payment

## Steps to Reproduce
1. Log in as an authorized account.
2. Open the payment page.
3. Enter card details.
4. Enter an invalid email value.
5. Click the payment confirmation button.
6. Review transaction logs or backend records.

## Expected Result
The invalid email should block submission and no transaction should be created.

## Actual Result
The UI shows an invalid email error, but the transaction still proceeds and fails in the backend.

## Severity
High

## Priority
High

## Business Impact
This causes bad user experience, unnecessary failed transactions, and inconsistent frontend versus backend behavior.

## Suggested Improvement
Prevent submission when frontend validation fails and add backend validation to reject malformed email values.
