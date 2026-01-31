# Ticket 20 – File Restore From Backup After Accidental Deletion

**Severity:** Medium  
**Category:** Backup / Recovery  
**Environment:** Lab – Windows Server 2022 File Server  

## Summary
A user accidentally deleted a critical file from a shared department folder and requested recovery.

## User Impact
The user temporarily lost access to important project notes stored on a shared file server.

## Initial Symptoms
- File missing from shared folder
- User confirmed accidental deletion

## Triage Summary
- Verified file deletion
- Confirmed backup availability
- Identified most recent valid copy

## Root Cause
The file was accidentally deleted by the user from the shared folder.

## Resolution
The file was restored from a known-good backup and validated with the user.

## Validation
- File successfully restored
- File contents verified
- User confirmed access

## Prevention
Backup awareness and safe file-handling practices were documented.

## Time to Resolve
Approximately 15–25 minutes

## Escalation Notes
Escalate if backups are unavailable or data cannot be restored.
