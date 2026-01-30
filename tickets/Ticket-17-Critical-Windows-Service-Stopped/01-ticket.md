# Ticket 17 – Critical Windows Service Stopped Unexpectedly

**Severity:** High  
**Category:** Monitoring / Services  
**Environment:** Lab – Windows Server 2022  

## Affected System
- **Server:** SRV-CORE01
- **Service:** Print Spooler

## Summary
A critical Windows service was found in a stopped state on a domain server, requiring investigation and restoration to ensure normal system functionality.

## User / System Impact
- Printing-related functionality was unavailable while the service was stopped.
- No additional system instability was observed.

## Initial Symptoms
- Print Spooler service was not running.
- No immediate error notifications presented to users.

## Triage Summary
- Verified service status in Services.
- Reviewed System logs for service-related events.
- Confirmed the service stopped cleanly without crashing.

## Root Cause
The Print Spooler service entered a stopped state due to a controlled stop event.

## Resolution
The affected service was restarted and confirmed running normally.

## Validation
Service status returned to running with no recurring failures.

## Prevention
Service monitoring and escalation criteria were documented.

## Time to Resolve
Approximately 10–15 minutes

## Escalation Notes
Escalate if the service repeatedly stops or fails to restart.
