# Security

## Introduction
This doc summarizes the security model and required controls.
Keep it current to reduce risk and audit effort.

## Threat model summary
- Unauthorized device access
- Data exfiltration
- Misconfigured permissions

## Authentication and authorization
- Devices authenticate with unique credentials.
- Users follow least privilege with role-based access.

## Data protection
- Encrypt data in transit and at rest.
- Separate tenant data logically.

## Secrets and keys
- Store secrets in a managed vault.
- Rotate keys on a defined schedule.

## Auditability
- Log privileged actions and configuration changes.
- Retain audit logs per policy.

## Security reviews
- Review new integrations before launch.
- Run periodic access audits.
