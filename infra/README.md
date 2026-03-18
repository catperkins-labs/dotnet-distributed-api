# infra

This directory will contain infrastructure-as-code and local development environment configuration.

## Planned Contents

- `docker-compose.yml` — one-command local dev environment (API, SQL Server, Redis, Orleans Silo)
- `bicep/` — Azure Bicep templates for cloud deployment (Azure SQL, Azure Cache for Redis, App Service / Container Apps)

## Usage

```bash
# Local dev
docker compose up

# Azure deployment
az deployment group create --template-file bicep/main.bicep
```
