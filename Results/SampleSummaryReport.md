# Sample Summary Report – NeoLoad Web + API Demo

## 1. Executive Summary

A conceptual performance test was executed to validate the behavior of a web + API application under load. The test focused on login, dashboard, and account detail operations.

## 2. Test Scenario

- 500 concurrent users
- 60-minute steady-state
- Mixed user journeys

## 3. SLA Results (Example Data)

- Login: 95th percentile = 2.4 sec (SLA: 3 sec) – ✅
- Dashboard: 95th percentile = 3.8 sec (SLA: 4 sec) – ✅
- View Account: 95th percentile = 2.9 sec (SLA: 3 sec) – ✅

## 4. Observations

- Throughput increased linearly with user load up to ~400 users.
- At 500 users, minor increase in response times observed.

## 5. Bottleneck Analysis (Conceptual)

- APM traces indicated occasional delays on the accounts API due to DB connection pool saturation.
- Recommendation: review connection pool sizing and DB query performance.

## 6. Recommendations

- Tune DB connection pool sizing.
- Consider indexing adjustments on high-frequency queries.
- Re-test after tuning to confirm improvements.
