# Ticket-15-Windows-Update-Failure/01-ticket.md

# Ticket 15 – Windows Update Failing on Client

**Severity:** Medium  
**Category:** Endpoint / Updates  
**Environment:** Lab – Windows 11 Pro Client  

## Affected User
- **User:** ben jones
- **Workstation:** WIN11-02

## Summary
A user reported that Windows Updates were failing to complete on their workstation. Update checks would hang or fail, preventing the system from receiving updates.

## User Impact
- System updates could not be verified or installed.
- Potential risk of missing security and stability updates.

## Initial Symptoms
- Windows Update failed or stalled during update checks.
- No system crash or network outage observed.

## Triage Summary
- Observed update failure behavior in Settings.
- Verified update-related service status.
- Reviewed system logs for update-related errors.

## Root Cause
Windows Update service behavior was inconsistent, preventing update checks from completing successfully.

## Resolution
Required update-related services were verified and restored, allowing Windows Update to resume normal operation.

## Validation
Windows Update successfully completed an update check without errors.

## Prevention
Update service monitoring and escalation criteria were documented.

## Time to Resolve
Approximately 15–20 minutes

## Escalation Notes
Escalate if update failures persist, recur frequently, or affect multiple systems.
