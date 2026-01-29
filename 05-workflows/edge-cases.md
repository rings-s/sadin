# Edge Cases

## Introduction
This doc captures tricky scenarios so we handle them consistently.
Add cases whenever we see production surprises.

## Known edge cases
- Device clock drift leads to out-of-order data.
- Duplicate telemetry events on retries.
- Ingestion burst after connectivity restore.
- Invalid schema versions in the field.
- Missing metadata for newly provisioned devices.

## Expected behavior
- System should be resilient and fail safely.
- Operators should see clear alerts and remediation steps.
