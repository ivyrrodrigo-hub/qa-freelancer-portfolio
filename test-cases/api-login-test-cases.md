# API Login Test Cases

## Scope
Validation of a login/authentication API.

## Sample Test Cases

| Test Case ID | Scenario | Steps | Expected Result |
|---|---|---|---|
| TC-API-001 | Valid login request | Send request with valid credentials | API returns success response and token |
| TC-API-002 | Invalid password | Send request with wrong password | API returns authentication error |
| TC-API-003 | Missing required field | Omit password from request body | API returns validation error |
| TC-API-004 | Unauthorized access | Call protected endpoint without token | API returns 401 Unauthorized |
| TC-API-005 | Invalid method | Call endpoint using unsupported HTTP method | API returns proper method error |
| TC-API-006 | Response schema validation | Send valid request | Response matches expected structure |

## Validation Focus
- status code
- response body
- authentication behavior
- error handling
- schema consistency
