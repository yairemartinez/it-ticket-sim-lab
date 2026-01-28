# Ticket 11 – User Cannot Access File Server (Network Path Issue)

**Severity:** Medium  
**Category:** Networking / File Services  
**Environment:** Lab – Windows Server 2022 File Server, Windows 11 Pro Client  

## Summary
A user was unable to access a departmental file share using the server hostname, while access by IP address remained functional.

## User Impact
The user temporarily lost access to shared departmental files when using the standard network path.

## Initial Symptoms
- Access to `\\SRV-CORE01\DeptShare` failed
- Access to `\\10.0.0.10\DeptShare` succeeded
- Network drives intermittently disappeared from File Explorer

## Triage Summary
- Tested hostname vs IP-based access
- Verified SMB connectivity
- Reviewed client DNS configuration

## Root Cause
Incorrect client-side DNS configuration prevented reliable hostname resolution to the file server.

## Resolution
The client DNS configuration was corrected to use the internal domain DNS server.

## Validation
File server access via hostname was restored and network drives reappeared consistently.

## Prevention
DNS configuration standards for domain-joined systems were documented.

## Time to Resolve
Approximately 20–30 minutes

## Escalation Notes
Escalate if multiple users experience file server access failures.
