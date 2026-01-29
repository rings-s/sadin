# Data Model

## Introduction
This doc describes the core data model and shared conventions.
Use it to keep naming, keys, and retention consistent.

## Canvas
Open: [[Data Model.canvas]]

## Core entities
- Tenant
- Device
- DeviceType
- TelemetryEvent
- Alert
- User

## Key conventions
- Use snake_case for column names.
- Primary keys are UUIDs unless noted.
- Timestamps use UTC.

## Partitioning and retention
- Partition telemetry by time and tenant.
- Retention defaults to 90 days unless configured.

## Data ownership
| Data set | Owner | Notes |
| --- | --- | --- |
| Telemetry | Data | High volume |
| Config | Platform | Low volume |
