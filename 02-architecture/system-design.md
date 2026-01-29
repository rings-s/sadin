# System Design

## Introduction
This doc describes the system at a high level and how parts fit together.
It should be understandable to product, engineering, and ops alike.

## Canvas
Open: [[system-design.canvas]]

## High-level components
- Device layer: physical devices and firmware
- Ingestion service: receives and validates telemetry
- Processing service: transforms and enriches data
- Storage layer: time-series and relational data stores
- API layer: internal and external access
- Observability: logs, metrics, and tracing

## Component responsibilities
- Ingestion: authentication, validation, rate limiting
- Processing: normalization, routing, alert evaluation
- Storage: persistence, indexing, retention
- API: query, management, and reporting

## Data stores
| Store | Purpose | Retention | Owner |
| --- | --- | --- | --- |
| Time-series DB | Telemetry | 90 days | Data |
| Relational DB | Users, devices, config | 1 year+ | Platform |

## Interfaces
- Device protocol endpoints
- Admin and operator APIs
- Webhooks for integrations

## Key risks
- Ingestion spikes during outages
- Schema changes impacting older devices
- Cost growth with high-frequency telemetry
