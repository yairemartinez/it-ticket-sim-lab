# Ticket-14-Client-Disk-Space-Alert/01-ticket.md

# Ticket 14 – Disk Space Alert on Client Machine

**Severity:** Low  
**Category:** Endpoint / Storage  
**Environment:** Lab – Windows 11 Pro Client  

## Affected User
- **User:** ben jones  
- **Workstation:** WIN11-01  

## Summary
The user reported receiving low disk space warnings on their workstation. The system drive (C:) was nearly full, triggering Windows alerts and requiring investigation.

## User Impact
- Low disk space warnings displayed.
- Potential impact to system performance and updates.

## Initial Symptoms
- C: drive displayed as low disk space.
- Windows issued a low disk space warning.

## Triage Summary
- Verified disk usage on the system drive.
- Identified large non-essential files consuming disk space.

## Root Cause
Insufficient free disk space on the system drive caused by large user-level files.

## Resolution
Unnecessary files were safely removed, restoring available disk space.

## Validation
Disk space returned to normal operating levels and warnings cleared.

## Prevention
Disk usage best practices and cleanup guidance were documented.

## Time to Resolve
Approximately 15–20 minutes

## Escalation Notes
Escalate if disk space cannot be reclaimed through cleanup or if repeated alerts occur.
