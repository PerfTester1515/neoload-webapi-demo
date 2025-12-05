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

Store it in a variable (e.g., ${auth_token}).
