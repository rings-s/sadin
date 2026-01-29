# Data Validation

## Introduction
This doc describes how we validate and clean incoming data.
It protects downstream systems and analytics.

## Validation steps
- Authenticate device identity.
- Validate schema version and required fields.
- Enforce type and range checks.
- Normalize units and timestamps.

## Error handling
- Reject invalid payloads with clear reasons.
- Store failed events in a dead-letter queue.
- Provide dashboards for validation failures.

## Schema versioning
- Backward compatibility is the default.
- Breaking changes require a migration plan.
