# Data Flow

## Introduction
This doc shows how data moves through the system end to end.
Use it when troubleshooting latency or data quality issues.

## Canvas
Open: [[data-flow.canvas]]

## Happy path
1. Device authenticates and sends telemetry.
2. Ingestion validates schema and rate limits.
3. Processing normalizes and enriches data.
4. Storage persists data with correct retention.
5. Alerts trigger and notify operators.
6. APIs and dashboards display results.

## Error handling
- Invalid payloads are rejected with clear reasons.
- Retries use backoff and are capped.
- Dead-letter queue stores rejected events.

## Data contracts
- Every payload has a versioned schema.
- Changes require backward compatibility or migration.
