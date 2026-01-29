# Deployment

## Introduction
This doc defines how we deploy safely and repeatably.
Keep it in sync with CI/CD pipelines.

## Pre-flight checklist
- Tests passing and changelog updated.
- Monitoring and alerts confirmed.
- Rollback plan documented.

## Deployment steps
1. Announce deployment window.
2. Deploy to staging and validate.
3. Deploy to production.
4. Monitor critical metrics.

## Rollback
- Trigger rollback if SLOs degrade.
- Notify stakeholders and update incident log.
