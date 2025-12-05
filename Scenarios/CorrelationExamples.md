# Correlation Strategy – NeoLoad Web + API Demo

## Example 1 – Auth Token

- **Request:** `POST /api/auth/login`
- **Response:** Contains a JSON Web Token (JWT) in the response body:
  ```json
  {
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9..."
  }

Approach:
Use a NeoLoad extractor to capture the token value from the JSON response.
Store it in a variable (e.g., ${auth_token})

## Example 2 – Dynamic Account ID

- **Request:** `GET /api/accounts`
- **Response:** ` Returns a list of account IDs in JSON.`
Extract one or more account IDs using a JSON or regexp extractor.
Use NeoLoad variable policies to:
Randomly choose an account
Or iterate through multiple accounts

## General Guidelines
Always correlate values that:
  
  Are generated at runtime
  
  Appear in multiple requests (tokens, session IDs, dynamic IDs)

Validate correlation via:
  Debug logs
  NeoLoad validation mode
