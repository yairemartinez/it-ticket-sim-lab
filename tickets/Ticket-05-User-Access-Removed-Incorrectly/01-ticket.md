# Ticket 05 – User Access Removed Incorrectly

**Severity:** Medium  
**Category:** Access / Authorization  
**Environment:** Lab – Windows Server 2022 File Share, Windows 11 Pro Client  

## Summary
A user reported losing access to a shared folder they previously had access to.

## User Impact
The user could not access files required for daily work.

## Initial Symptoms
The user received an “Access Denied” error when accessing a previously available folder.

## Triage Summary
- Verified share availability
- Reviewed user group membership

## Root Cause
The user was removed from the security group controlling access to the shared folder.

## Resolution
The user was restored to the appropriate security group.

## Validation
Access to the shared folder was successfully restored.

## Prevention
Group-based access management practices were reinforced.

## Time to Resolve
Approximately 15–20 minutes

## Escalation Notes
Escalate if access removal was unauthorized or impacts multiple users.

