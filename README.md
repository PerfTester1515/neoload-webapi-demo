# NeoLoad Web + API Demo Project

This repository contains a conceptual NeoLoad performance testing project designed to demonstrate my approach to testing a modern web + API application.

> Note: This project uses placeholder structures and documentation only. No client or proprietary assets are included.

## Objectives

- Model a typical user journey through a web application backed by REST APIs.
- Demonstrate how I think about correlation, parameterization, SLAs, and workload design.
- Show how I structure performance test documentation and results in a repeatable way.

## System Under Test (Conceptual)

- **Front-end:** Web UI (login, dashboard, account details, logout)
- **Back-end:** REST APIs for authentication, account summary, and transactions
- **Environment:** Typical 3-tier architecture (Web → App → DB)

## Repository Layout

- `TestPlan/` – Performance test plan and workload model
- `Scenarios/` – User journeys and examples of correlation/parameterization strategy
- `Data/` – Sample test data files (CSV format)
- `Results/` – Example summary + findings structure
- `Docs/` – Notes on NeoLoad configuration and project setup

## Key Concepts Demonstrated

- Designing user journeys for NeoLoad
- Correlation strategy (dynamic tokens, session IDs, etc.)
- Parameterization strategy for more realistic data
- Defining SLAs and success criteria
- Organizing results and findings for stakeholders

## About Me

I am a Senior Performance Engineer with 15+ years of experience using tools such as LoadRunner, NeoLoad, Gatling, Dynatrace, AppDynamics, Splunk, and various messaging and database technologies.

This repo is intended to provide a high-level view of how I structure and communicate performance testing efforts using NeoLoad.
