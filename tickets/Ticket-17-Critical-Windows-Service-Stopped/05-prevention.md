# Prevention – Preventing Service Outages

## Prevention Steps
- Monitor critical services for unexpected state changes.
- Review System logs regularly for Service Control Manager events.
- Address service interruptions promptly to prevent impact to dependent functionality.

## Operational Notes
- Event ID 7036 indicates a controlled service state change.
- Repeated or unexpected service stops may indicate deeper issues.
- Core services should be included in monitoring and alerting workflows.

## Escalation Criteria
Escalate to systems administration if:
- The service stops repeatedly.
- The service fails to restart.
- Additional dependent services are impacted.
