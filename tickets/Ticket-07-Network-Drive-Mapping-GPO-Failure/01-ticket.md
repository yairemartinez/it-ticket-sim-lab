# Ticket 07 – Network Drive Mapping via GPO Fails

**Severity:** Medium  
**Category:** Group Policy / File Access  
**Environment:** Lab – Windows Server 2022 AD DS, Windows 11 Pro Client  

## Summary
A network drive mapping configured via Group Policy did not appear for a user.

## User Impact
The user could not access departmental files via the expected mapped drive.

## Initial Symptoms
The mapped drive was missing after login.

## Triage Summary
- Verified GPO application
- Verified network path access
- Reviewed GPO targeting

## Root Cause
The drive mapping did not apply due to user session timing and Group Policy processing context.

## Resolution
A Group Policy update was forced and the user session was refreshed.

## Validation
The network drive mapped successfully after re-login.

## Prevention
Drive mapping best practices were documented.

## Time to Resolve
Approximately 15 minutes

## Escalation Notes
Escalate if drive mappings fail across multiple users or OUs.

