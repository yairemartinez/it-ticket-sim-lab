# Ticket 08 – Group Policy Causes Login Delay

**Severity:** Medium  
**Category:** Group Policy / Performance  
**Environment:** Lab – Windows Server 2022 AD DS, Windows 11 Pro Client  

## Summary
A user experienced slower login times following the introduction of a new user-scoped Group Policy Object.

## User Impact
Increased login time affected the user experience during daily system access.

## Initial Symptoms
User reported delays during login while applying user settings.

## Triage Summary
- Reviewed applied Group Policy Objects
- Identified broad GPO scope affecting all users

## Root Cause
User policies were linked at a high-level OU, increasing logon processing overhead.

## Resolution
The GPO scope was reduced by linking it only to the appropriate Users OU.

## Validation
The policy continued to apply correctly, and login performance improved.

## Prevention
GPO scoping best practices were documented to prevent similar performance issues.

## Time to Resolve
Approximately 20–30 minutes

## Escalation Notes
Escalate if login delays affect multiple users or persist after scope optimization.
