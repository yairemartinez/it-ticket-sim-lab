# Ticket 19 – Accidental Deletion of AD User Object

**Severity:** High  
**Category:** Active Directory / Recovery  
**Environment:** Lab – Windows Server 2022 AD DS  

## Summary
A domain user account was accidentally deleted and required recovery.

## User Impact
The user could not authenticate or access domain resources.

## Initial Symptoms
User login failed and account was missing from Active Directory.

## Triage Summary
- Verified user deletion
- Reviewed deleted objects

## Root Cause
User account was accidentally deleted.

## Resolution
User account was restored using Active Directory Recycle Bin.

## Validation
User authentication and access restored.

## Prevention
Directory change control practices were documented.

## Time to Resolve
Approximately 15–20 minutes

## Escalation Notes
Escalate if multiple directory objects are deleted.

