# Ticket 09 – Security Policy Change Causes Login Failure

**Severity:** High  
**Category:** Group Policy / Security  
**Environment:** Lab – Windows Server 2022 AD DS, Windows 11 Pro Client  

## Summary
A recent security policy change prevented users from logging in.

## User Impact
Users were unable to access their workstations.

## Initial Symptoms
Login attempts failed following a policy update.

## Triage Summary
- Reviewed applied Group Policies
- Identified recent security policy change

## Root Cause
A misconfigured security policy denied users the ability to log on locally.

## Resolution
The security policy was rolled back to restore access.

## Validation
Users were able to log in successfully after rollback.

## Prevention
Change control and testing procedures were documented.

## Time to Resolve
Approximately 30–45 minutes

## Escalation Notes
Escalate if login failures affect multiple systems or users.
