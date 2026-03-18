# load-tests

This directory will contain k6 load test scripts for performance and stress testing the API.

## Planned Contents

- Ramp-up scripts targeting key endpoints (e.g., event ingestion, aggregate queries)
- Scenarios for sustained load (e.g., 500 RPS) and spike testing
- Summary of p50 / p95 / p99 latency results

## Usage

```bash
k6 run scripts/smoke.js
k6 run scripts/ramp.js
```
