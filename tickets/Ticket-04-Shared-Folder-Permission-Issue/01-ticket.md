# Ticket 04 – User Cannot Access Shared Folder

**Severity:** Medium  
**Category:** Access / File Services  
**Environment:** Lab – Windows Server 2022 File Share, Windows 11 Pro Client  

## Summary
A user reported being unable to access a required shared folder.

## User Impact
The user could not access departmental files needed for daily work.

## Initial Symptoms
The user received an “Access Denied” error when accessing the shared folder.

## Triage Summary
- Verified network connectivity
- Reviewed share and NTFS permissions

## Root Cause
NTFS permissions did not include the user’s security group, preventing access despite permissive share permissions.

## Resolution
The appropriate security group was added to the NTFS permissions with least-privilege access.

## Validation
The user successfully accessed and modified files in the shared folder.

## Prevention
Group-based permission management was documented to prevent similar issues.

## Time to Resolve
Approximately 15–25 minutes

## Escalation Notes
Escalate if access requirements are unclear or affect multiple users.

