# Non-Functional Requirements

## Introduction
This doc defines quality targets and system characteristics.
These targets guide architecture and testing.

## Targets
| Category | Target | Notes |
| --- | --- | --- |
| Availability | 99.9% monthly | Excluding planned maintenance |
| Latency | P95 under 5s | From device ingest to availability |
| Throughput | Scales with fleet size | Load test before release |
| Security | Least privilege | Audited access |
| Data retention | Configurable | Per customer policy |

## Measurement
- Track metrics in dashboards under `07-operations/monitoring.md`.
- Review against targets each sprint review.
