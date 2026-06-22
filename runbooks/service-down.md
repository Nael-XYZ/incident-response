# Service Down Runbook

## Detection
- Alert: "Service X is not responding"
- Dashboard shows 5xx spike

## Triage
1. Check if deploy happened in last 30min
2. Check pod/node status
3. Check dependency health

## Mitigation
- If deploy-related: rollback
- If infra: restart pods
- If dependency: circuit break

## Post-mortem
- Timeline of events
- Root cause
- Action items
