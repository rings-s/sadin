# Entities

## Introduction
This doc lists the primary entities and their key fields.
Keep fields stable and document changes in the decision log.

## Tenant
- id, name, status, created_at

## Device
- id, tenant_id, device_type_id, status, last_seen_at

## DeviceType
- id, name, firmware_version, protocol

## TelemetryEvent
- id, device_id, received_at, payload, schema_version

## Alert
- id, device_id, severity, message, created_at

## User
- id, tenant_id, role_id, email, status
