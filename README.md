# Pulse Desk

> A production-minded operations workspace for teams that need a clear view of clients, work items, ownership, and service health.

## The problem

Operational teams often manage client requests, priorities, and follow-ups across disconnected tools. That creates unclear ownership, weak visibility into work in progress, and little historical context for decisions.

Pulse Desk centralizes that workflow in one focused product: clients, tasks, responsibilities, status changes, and meaningful operational metrics.

## Product direction

- **Role-aware workspace** for collaborators and managers
- **Client and work-item management** with ownership, priority, status, and history
- **Operational dashboard** for workload, cycle time, and blocked work
- **Audit-friendly activity trail** for key changes
- **API-first design** to support integrations and future automation

## Architecture

```text
Next.js web application
          │
          ▼
NestJS REST API ─── PostgreSQL
          │
          ├──── Redis cache
          └──── Background jobs and event processing
```

## Engineering standards

- Type-safe contracts with TypeScript
- Validation and clear error responses at API boundaries
- Relational data modelling with PostgreSQL
- Docker-based local environment
- Tests for business rules and integration points
- Structured logs, API documentation, and CI checks as the product evolves

## Technology

| Area | Choice |
| --- | --- |
| Web | Next.js, React, TypeScript |
| API | NestJS, TypeScript, REST |
| Data | PostgreSQL |
| Async & cache | Redis and queues |
| Environment | Docker |
| Quality | Jest, OpenAPI, GitHub Actions |

## Delivery plan

The first release focuses on authentication, roles, clients, tasks, and dashboard metrics. The next iterations add event processing, observability, and deployment automation.

## Status

Active development. The repository currently contains the product foundation and local environment definition; features are delivered incrementally with documentation and tests.

