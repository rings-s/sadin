# Environments

## Introduction
This doc explains our environments and how they differ.
It prevents accidental changes in the wrong place.

## Environments
| Environment | Purpose                   | Data policy    | Access      |
| ----------- | ------------------------- | -------------- | ----------- |
| Dev         | Local and feature testing | Synthetic data | Engineering |
| Staging     | Pre-prod validation       | Masked data    | Eng + Ops   |
| Prod        | Customer traffic          | Real data      | Restricted  |

## Rules
- Never use prod data in dev.
- Changes in prod require approval.
