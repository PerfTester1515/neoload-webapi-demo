---

### 🔹 `Scenarios/ParameterizationExamples.md`

```markdown
# Parameterization Strategy – NeoLoad Web + API Demo

## Data Files

- `Data/users.csv`
  - Columns: `username,password`
- `Data/accounts.csv`
  - Columns: `account_id`

## Approach

- Use NeoLoad variables to read from CSV files.
- Configure policies:
  - Unique per user (for login usernames)
  - Random for account IDs
  - Reuse on error vs. move to next row, depending on test type.

## Goals

- Avoid reusing the same user for all virtual users.
- Simulate more realistic data access patterns.
- Prevent caching effects from masking performance issues.

