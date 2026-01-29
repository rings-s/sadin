# Monitoring

## Introduction
This doc defines what we monitor and why.
Good monitoring keeps us proactive instead of reactive.

## Canvas
Open: [[monitoring.canvas]]

## Key signals
- Ingestion rate and error rate
- Processing latency
- Alert delivery success
- Storage saturation

## SLOs
- Availability: 99.9% monthly
- Latency: P95 under 5s

## Alert routing
- Sev1: On-call immediately
- Sev2: On-call within 30 minutes
- Sev3: Daily review
