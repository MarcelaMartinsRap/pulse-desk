# Pulse Desk

An operations dashboard for tracking clients, work items, and service metrics.

## Why it exists

Pulse Desk is a portfolio project designed around real product concerns: authentication, role-based access, client and task management, REST APIs, metrics, auditability, and maintainable architecture.

## Planned stack

- **Web:** Next.js and TypeScript
- **API:** NestJS and TypeScript
- **Data:** PostgreSQL
- **Performance & asynchronous work:** Redis and background queues
- **Environment:** Docker

## First release scope

1. Authentication and user roles.
2. Clients and tasks with status, priority, and ownership.
3. An operations dashboard with practical metrics.
4. Change history and documented APIs.

## Engineering goals

The project is intentionally built to demonstrate data modelling, API design, business rules, tests, observability, and technical decisions that can evolve with the product.

## Status

Foundation in progress. The first milestone is a NestJS health endpoint backed by a local PostgreSQL environment.
