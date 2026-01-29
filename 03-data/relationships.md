# Relationships

## Introduction
This doc shows how entities relate to each other.
Use it when planning migrations or reporting needs.

## Relationships
- Tenant 1..* Device
- Device 1..* TelemetryEvent
- Device 1..* Alert
- Tenant 1..* User
- DeviceType 1..* Device

## Rules
- Deletes are soft by default.
- Cascades must be explicit and reviewed.
