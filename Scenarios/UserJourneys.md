# User Journeys – NeoLoad Web + API Demo

## Journey 1 – Standard User

1. Open Login Page
2. Submit credentials (`POST /api/auth/login`)
3. Load dashboard (`GET /api/accounts`)
4. View first account (`GET /api/accounts/{id}`)
5. Logout

## Journey 2 – Power User

1. Login
2. Load dashboard
3. Iterate through several accounts (`GET /api/accounts/{id}`)
4. Logout

## Journey 3 – Quick Check

1. Login
2. Load dashboard
3. Logout

Each of these user paths would be scripted in NeoLoad as separate User Paths, with shared correlation and parameterization logic.
