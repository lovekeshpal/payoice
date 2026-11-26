# ADR-001: Tech stack

## Status
Accepted, 25 Nov 2026

## Context
Payoice needs a stack that a small team can build, test and
deploy quickly, with strong support for AI features.

## Decision
Angular frontend, Python FastAPI backend, PostgreSQL,
Docker, GitHub Actions, Google Cloud Run.

## Why
- Angular: mature, typed frontend framework with Signals
- FastAPI: async, Pydantic validation, automatic API docs
- Python: where the best AI libraries ship first
- PostgreSQL: transactions for money, pgvector later
- Cloud Run: scales to zero, low cost at small scale

## Rejected
- Node.js backend: Python has stronger AI libraries
- MongoDB: money needs strict relations and transactions
- Kubernetes: overkill at this stage