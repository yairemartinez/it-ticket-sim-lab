# Ticket 04 – User Cannot Access Shared Folder

**Severity:** Medium  
**Category:** Access / File Services  
**Environment:** Lab – Windows Server 2022 File Share, Windows 11 Pro Client  

## Summary
A user reported being unable to access a required shared departmental folder due to permission misconfiguration.

## User Impact
The user could not access departmental files needed to perform daily work tasks.

## Initial Symptoms
The user received an “Access Denied” error when attempting to access the shared folder.

## Triage Summary
- Verified network connectivity to the file server.
- Reviewed share and NTFS permissions on the affected folder.

## Root Cause
The access issue was caused by a mismatch between share and NTFS permissions. NTFS permissions initially did not include the user’s security group, and the existing share permissions were overly restrictive, resulting in insufficient effective access.

## Resolution
The appropriate security group was added to the NTFS permissions with Modify access. Share permissions were updated to ensure they supported the intended level of NTFS access while maintaining least-privilege principles.

## Validation
The user successfully accessed the shared folder and was able to create and modify files as expected.

## Prevention
Group-based permission management was documented, and both share and NTFS permissions are now reviewed together to prevent similar access issues.

## Time to Resolve
Approximately 15–25 minutes.

## Escalation Notes
Escalate if access requirements are unclear, undocumented, or if the issue affects multiple users or groups.
