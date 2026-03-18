# dotnet-distributed-api

A high-performance distributed backend showcase using .NET 9, Orleans, Dapper, SQL Server, and Redis.

## Projects

| Project | Type | Purpose |
|---|---|---|
| `src/Api` | ASP.NET Core Web API | HTTP host — exposes REST endpoints to clients |
| `src/Core` | Class Library | Domain models and interfaces; no external dependencies |
| `src/Data` | Class Library | Dapper-based data access layer for SQL Server |
| `src/Caching` | Class Library | Redis and IMemoryCache abstraction (L1/L2 cache pattern) |
| `src/Grains` | Class Library | Orleans grain interfaces and implementations |
| `src/Silo` | Console App | Orleans silo host |
| `tests/UnitTests` | xUnit Test Project | Unit tests for Core, Data, Caching, and Grains |
| `tests/IntegrationTests` | xUnit Test Project | Integration tests using Testcontainers (SQL Server + Redis) |

## Technologies

| Technology | Role |
|---|---|
| C# / .NET 9 | Primary language and runtime |
| ASP.NET Core | REST API host |
| Orleans | Distributed actor framework for grain-based state |
| Dapper | Lightweight, high-performance SQL data access |
| SQL Server | Primary relational data store |
| Redis | Distributed cache |
| xUnit | Unit and integration test framework |
| Testcontainers | Spin up real SQL Server and Redis containers for integration tests |
| k6 | Load testing and performance benchmarking |
| Docker | Local development environment via Docker Compose |
| Azure Bicep | Infrastructure-as-code for Azure deployments |

## Getting Started

> Setup instructions coming in a future phase. See `infra/README.md` for the planned Docker Compose setup.

## Architecture

> Architecture diagram and detailed design notes coming in a future phase.

## Load Testing

> k6 load test scripts and results coming in a future phase. See `load-tests/README.md`.

## Infrastructure

> Azure Bicep templates and Docker Compose configuration coming in a future phase. See `infra/README.md`.
